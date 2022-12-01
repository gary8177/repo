Matrix 首页推荐

[Matrix](https://sspai.com/matrix) 是少数派的写作社区，我们主张分享真实的产品体验，有实用价值的经验与思考。我们会不定期挑选 Matrix 最优质的文章，展示来自用户的最真实的体验和观点。

文章代表作者个人观点，少数派仅对标题和排版略作修改。

* * *

本文主要介绍 Windows 系统下的符号链接（Symbolic Link）和硬链接（Hard Link）的原理，特性以及它们在日常工作生活中应用。

这两类链接直接由文件系统实现和支持，各类软件无需适配即可使用。学会使用这两种链接，我们就可以：

-   用云盘保存那些不方便改变位置的文件
-   使用完全不同的路径编辑同一个文件
-   实现更省空间的增量备份

## 初识符号链接与硬链接

如果你对这两个名字感到陌生，那么可以打开你的系统盘，在根目录使用 Shift + 右键的方式进入 PowerShell，键入 `dir -force` 来列出所有的文件和文件夹。其中一定会有名为 `Documents and Settings` 的文件夹，在名称后面有一个箭头指向了 `C:\Users`。该文件夹的作用是：当应用想要访问 `C:\Documents and Settings` 这个路径时，系统会自动将它引导到 `C:\Users`，应用可以用 Documents and Settings 这个目录名访问 Users 下的任何内容。

这是微软为了保证 Windows Vista 以前的应用仍然能够正确安装在 Windows 10 上所做的设计，此文件夹正类似 1

被称为目录链接（Junction），它和符号链接原理和效果都类似，但仅能用于本地卷的目录。本文不做过多介绍。读者可以泛泛地将它理解为符号链接。

于符号链接。

![](https://cdn.sspai.com/2021/07/09/article/75533f03740ae44ce91aacc92552d0c6?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

硬链接就没这么麻烦，因为文件管理器上的几乎所有文件都可以被看作是硬链接。不信的话可以在终端中使用系统内置的硬链接查询命令：`fsutil hardlink list [文件路径]`。它会列出一个文件对应的所有的硬链接路径，该工具一定会给出的此文件本身的路径。

![](https://cdn.sspai.com/2021/07/09/article/e9f853784b04e42f2d09f5e793433d5a?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

和这两类链接见了面之后，我们还要重新认识一下「文件」。

在一台 Windows 电脑中，硬盘被分割为卷用以保存数据，在每一个卷上，数据对象被 NTFS 文件系统赋予了独一无二的**文件 ID** 以及**与之对应的文件路径**，文件路径和文件 ID 对应，文件 ID 和数据对象绑定，最终才呈现为可供用户打开、编辑的文件。

因此可以说，我们所看到的文件并非数据本身，而是由文件路径指向数据对象的链接。

本文的主角，符号链接和硬链接正和这种数据的组织方式息息相关。

## 符号链接的原理和特性

前面说道，文件是数据对象和文件路径的链接，符号链接则是将自己链接到一个目标文件或目录的路径上。当系统识别到符号链接时，它会跳转到符号链接所指向的目标中去，而不改变此时的文件路径。

![](https://cdn.sspai.com/2021/07/09/article/250035488b0e9a44e46f3115295461e0?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

举例来说，有一个名为 source 的文件夹。在桌面使用管理员权限打开 PowerShell，输入 `New-Item Symlink -ItemType SymbolicLink -Target C:\...\source` 为 source 文件夹创建名为 Symlink 的符号链接。然后打开此新建的文件夹，可以发现虽然路径是 Desktop\\Symlink，但无论是内部的目录结构还是文件内容，都和 source 文件夹一模一样。

![](https://cdn.sspai.com/2021/07/09/article/67abff5f10c1673f93927b8873c43bd7?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

符号链接像一个虫洞：当用户或应用要访问此虫洞时，就会被传送到符号链接所指向的地方，**但他们是通过虫洞访问此目标的**，所以其路径仍是虫洞自己的路径，这是它和快捷方式在效果上的区别所在。

更进一步说，符号链接的名称或者后缀丝毫不会影响到其目标。如果有一个图片 cats.jpg，我为它创建一个叫做 cats.docx 的符号链接，双击 cats.docx 时，仍然会出现一个图片。

![](https://cdn.sspai.com/2021/07/09/article/4294a3a2303768570c51e827c380295a?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

符号链接具有下面的特性：

-   **只需要一个路径。** 创建时，它的目标可以是本地的、远程的任何文件或目录，即使目标不存在。
-   **所做的一切更改都会反映在目标上**。因为打开符号链接，就是打开了目标。复制符号链接，会复制目标的内容；移动符号链接，则会移动链接本身。
-   更改目标的名称，移动目标的位置，符号链接将会成为死链，因为它无法通过设定的路径找到目标；更改符号链接本身的名称和位置，目标不受影响。
-   当目标被删除时，符号链接继续存在，但会成为死链，无法打开。当符号链接被删除时，它指向的目标不受影响。

## 硬链接的原理和特性

硬链接和符号链接的原理完全不同，符号链接是指向目标路径的链接，而硬链接则是指向目标数据对象的链接。因为一个卷中的数据对象都有一个独一无二文件 ID，也可以说硬链接是指向目标文件 ID 的链接。

不难发现，硬链接和前面对文件的定义是一样的，原因在于，同一个文件 ID 可以对应很多 2

很多，但小于 1024 个。即最多有 1023 个硬链接指向同一文件 ID。因此，第七节中提到的 DeLorean Copy 一般情况下最多只能有 1023 个备份

不同的文件路径。这些不同的文件都可以被称为 3

理论如此，但为了避免混淆，本文按习惯称文件 ID 只与一个文件路径对应的为文件。仅有多个对应关系的才称之为硬链接。

硬链接。这也是为什么在第一节中说「文件管理器上的几乎所有文件都可以被称为硬链接」。

![](https://cdn.sspai.com/2021/07/09/article/8e2c1ee82f4917a9d07c4d5a7ce9f809?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

这里之所以引入文件 ID 的概念，是因为通过它我们可以直观看到文件所指的数据是否改变。以桌面上的 Demo.txt 为例，使用 `fsutil file queryFileID Demo.txt` 可以查看到它对应的文件 ID 为 `...3d321`。当我们用复制粘贴的方式为此文件创建一个副本 Demo - Copy.txt 时，通过 ID `...5d78c` 可知我们实际上创建了另一个数据。

![](https://cdn.sspai.com/2021/07/09/article/27af80ae83c9a193398b53c83eb9b2d7?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

下面，在 PowerShell 中使用 `New-Item Hardlink.txt -ItemType HardLink -Target C:\...\Demo.txt` 给 Demo.txt 创建一个叫做 Hardlink.txt 的硬链接。同样用 `fsutil file queryFileID Hardlink.txt` 得到 Hardlink.txt 的文件 ID 为 `...3d321`，这和 Demo.txt 是一样的，说明两者都指向同一个数据对象。

![](https://cdn.sspai.com/2021/07/09/article/19ac322d2d570455bea2a8c2227b1dc9?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

因为他们数据是相通的，这两个文本所有属性都相同，更改其中一个文件的内容，另一个也会随之变化。

![](https://cdn.sspai.com/2021/07/09/article/d3da5706dd3e3e084a3c254f6f4cd27e?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

**由于不同的文件指向的是同样的数据，所以无论给同一个文件创建多少个硬链接，他们占整个卷的数据大小都是一样的**。下图中，当 C 盘只有一个大小为 4 G 的 ISO 文件时，剩余大小为 373 GB；我为此 ISO 创建了另外 4 个 硬链接之后，卷的剩余大小并不因此而变化，尽管属性界面显示他们为 20 GB。

![](https://cdn.sspai.com/2021/07/09/article/10b1d86df93ce4cf77643dd8aaed92b0?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

**硬链接可以看作是一个既有文件的别名**，它具有下面的特性：

-   创建时，它必须指向本地的同一个卷内存在的文件 4

    系统禁止用户创建目录硬链接。硬链接在指向文件夹会导致一个文件的父目录不唯一，系统在遍历文件夹内容时出现循环……

    ，在 C 盘创建硬链接只能指向 C 盘存在的文件。因为只有在同一个卷内，文件 ID 才是独一无二的，且没人能在这个卷内编辑另一个卷的数据。不存在的文件没有文件 ID。
-   打开硬链接，所做的一切更改都会反映在目标文件上。因为目标文件也链接着被更改的数据。
-   更改目标文件的名称、位置，硬链接不会受到影响。更改硬链接的名称、位置，目标文件不受影响，链接不会断开。因为改名，移动都不会改变文件 ID。
-   当目标被删除时，硬链接继续存在，且可以正常打开、编辑。因为他具备一个完整的文件结构。当硬链接被删除时，目标文件继续存在，不受影响。只有当一个文件 ID 对应的所有硬链接被删除时，数据才真正被标记为删除。

## 使用命令行或 Link Shell Extension 创建两种链接

新建符号链接和硬链接不像普通文件那样容易。第二、三节已经展示了使用 PowerShell 命令的方式来创建二者：

`New-Item [链接名称] -Itemtype SymbolicLink/HardLink -Target [目标绝对路径]`

新建符号链接始终需要管理员权限，`-target`后面一般说来需要填写绝对路径才能被识别。命令行创建的方式往往在脚本中更方便，对于普通用户而言，则有更简单、可视化的软件供选择。

Link Shell Extension 就是一个功能十分强大的符号链接、硬链接（以及没提到的目录链接）的新建和管理工具。使用 `choco install linkshellextension -y` 或者进入软件 [官网](https://schinagl.priv.at/nt/hardlinkshellext/hardlinkshellext.html)，下载安装包并打开。安装完成后，我们便能够使用鼠标中键或者右键来简单地创建链接。

打开文件管理器，选中作为目标的文件或者文件夹，按住鼠标中键，然后将它拖到想要创建链接的目标文件夹处，松开鼠标，就会弹出创建链接的快捷菜单，选择需要的选项即可创建完成。

![](https://cdn.sspai.com/2021/07/09/article/7e3befaea5a4013afa951c84f39e466e?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

另一种创建的方法是，选中一个文件或目录后，右键，点击 Pick Link Source，将其选择为目标。然后在另一个文件夹的空白处右键，在 Drop as 的子菜单中，选择需要创建的链接类型。

![](https://cdn.sspai.com/2021/07/09/article/583c19e9fd2bd6d131b6f80b199d8116?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

Link Shell Extension 自动为创建的链接添加特殊的标识，并且为其文件属性添加了诸如引用计数、符号链接目标等实用选项卡。

![](https://cdn.sspai.com/2021/07/09/article/e37364e1456f83d2008986a0a9b80af7?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

## 用例一：使用 OneDrive 实时保存微信重要文件

Windows 中有许多虽然关键但难以移动位置的文件夹，要想使用 OneDrive 等云盘保存他们，往往只能另外复制一份，但这又面临着源文件更新的问题。

举例来说，Windows 版微信会在文档中创建 WeChat Files 文件夹，其中有一个 File 目录包含了聊天中的已下载的各类文件，这个文件夹正是既重要又不太方便移动。

**而符号链接可以让任何文件夹以任何名称出现在另一个地方**，我们为此文件夹在 OneDrive 内创建一个符号链接，OneDrive 访问此链接时会被引导到微信的 File 文件夹内，其中的内容就会被全部上传到云端。

整个实现的过程也非常简单：打开微信的 File 文件夹和 OneDrive 云盘本地文件夹，使用 Link Shell Extension 拖动创建一个符号链接，完成！

![](https://cdn.sspai.com/2021/07/09/article/e0f1f8913fae278c0585c4c7bef6d601?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

这样做了之后，在本地打开 File 符号链接时，会展现微信文件夹中的数据。而在 OneDrive 云端上，Files 则被视作一个正常的文件夹。还可以用类似的方法备份 QQ 的接收文件夹，Windows Appdata 中的一些设置文件等等。需要注意的是，当目标文件删除或消失时，OneDrive 也删除你的备份。

**我们还可以考虑将上面的过程反过来**！将目标文件或目录放在 OneDrive 中，在需要的程序文件夹中创建符号链接。在上面的例子中，即在 OneDrive 中放一个 File 文件夹，把微信中的 File 数据移动到此文件夹中，然后在微信的 FileStorage 中创建以 OneDrive 的 File 为目标的符号链接。

这种做法好处是：程序卸载时只要提前将符号链接删除，就不必担心重要的文件会被卸载程序清除掉。

## 用例二：Hexo 和 Obsidian 文章实时同步

Hexo 是一个静态博客生成工具，Obsidian 则是一个本地笔记管理工具，这两个工具的库我都使用 Git 做版本管理。

因为博客文章常常就是笔记中的文章，所以正常情况下，我需要将笔记中写好的 Markdown 复制粘贴到 Hexo 的博客目录下，然后再发布。一份文本此时被分成了两个数据，一旦需要更改，还得在两边分别编辑。

既然这两个工具会使用到同一份文本，为什么不能使用硬链接将他们共同的 Markdown 连接在一起呢？

需要做的工作是，在为 Hexo 创建文章时，同时在 Obsidian 的笔记目录下创建这个文章的硬链接。由于两者数据相通，在 Obsidian 处的编辑会自动同步到 Hexo 端。示例脚本 New-Blog.ps1 如下：

    ## 计数作为文件名
    $count = [System.IO.Directory]::GetFiles("$home\Hexo\source\_posts").Count
    ## 提前写入 Markdown 的 yaml 头
    $date = Get-Date -Format "yyyy-MM-dd HH:mm:ss"
    $yaml = "---" + "`ntitle: $count" + "`ndate: '$date'" + "`nupdated: '$date'" + "`ncategories: []" + "`ntags: [blog]" + "`ndescription:" +"`n`n---"
    ## 在 Hexo 中创建文件
    Write-Output $yaml | Out-File $home\Hexo\source\_posts\$count.md
    ## 在 Obsidian 中创建硬链接
    New-Item $home\Note\$count.md -Type HardLink -Target $home\Hexo\source\_posts\$count.md
    ## 退出
    exit

配合几行简单的 AHK 脚本：

    #!N::
    run, "%USERPROFILE%\Program\New-Blog.ps1",,hide
    return

当按下 Win + Alt + N 时，就会静默运行脚本，同时新建博客和笔记。重命名和移动文件都不会改变文件 ID，因此，只要不删除，无论在 Obsidian 上怎么折腾都不会影响两者的同步关系。如果我不满意某篇博客，在 Hexo 删除了它，那么文本在 Obsidian 那里仍然留存。

在此例中，可能有人会问「为什么不用符号链接？」主要原因是 Obsidian 目前似乎有意 5

忽略掉笔记库的符号链接。另外，本例中的 Markdown 文件也比较适合使用硬链接。作为对比，Word 文档在编辑保存时原文件会被删除，替代以新文件，文件 ID 会改变，而这将导致链接失效。

其他复杂的文件格式或特殊的编辑器可能也有类似的情况。

## 用例三：DeLorean Copy 实现增量备份

创建硬链接相当于创建文件的别名，正如我在第三节演示的那样，它可以实现在不增加体积的情况下创建文件的副本，这个特性让它非常适合用来备份文件。事实上，macOS 的时间机器功能正是使用了硬链接。

而对于 Windows 用户而言，通过 Link Shell Extension 自带的 DeLorean Copy 功能即可实现增量备份和版本回溯。

简单来说，在第一次备份完毕后，假如该文件夹发生了更改，DeLorean Copy 会自动分析更改后的文件夹和前一次备份的文件夹的区别，相同的文件会被创建硬链接，新的文件会被复制，删除的文件则会被丢弃，由此就形成了第二个备份。 当然，这都由程序自动完成，用户需要做的只是选择需要备份的文件夹，中键拖放，选择 DeLorean Copy。

![](https://cdn.sspai.com/2021/07/09/article/f490810a0d9ddf2c182135bc77fe9f2d?imageView2/2/w/1120/q/40/interlace/1/ignore-error/1)

如果想要为这个增量备份创建自动任务，则可以使用 [ln.exe](https://schinagl.priv.at/nt/ln/ln.html) 这个由同开发者开发的命令行程序，将 `ln --delorean` 作为命令写入脚本，再参考 [Windows 本地自动化工具，任务计划程序应用举例](https://sspai.com/post/66129) 一文设置任务计划程序即可。

## 小结

本文以 Windows 为例介绍符号链接和硬链接的原理及应用，但这两类链接不只用于 Windows，它们在不同的操作系统上都有着广泛的支持。虽然实现的原理可能不太相同，但在应用层面也许有一些共通之处。

希望本文能够给你以启发。

首页推广题图来自 [Background vector created by rawpixel](https://www.freepik.com/vectors/background)

\> 下载少数派 [客户端 ](https://sspai.com/page/client)、关注 [少数派公众号 ](https://sspai.com/s/J71e)，了解更妙的数字生活 🍃

\> 想申请成为少数派作者？[冲！](https://sspai.com/apply/writing) 
 [https://sspai.com/post/66834](https://sspai.com/post/66834)
