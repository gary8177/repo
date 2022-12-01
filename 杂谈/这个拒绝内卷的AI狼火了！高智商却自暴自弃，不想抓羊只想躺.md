### 

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GD7j1XCLRkcjWicuM0ibXDLOkNPmJE45xcop8ia42YEH4bVRlLFuTXHhU2w/640?wx_fmt=png)

### 

* * *

**新智元报道**

来源：B 站等

编辑：Yaxin

##### **【新智元导读】** 近日，一个狼吃羊的 AI 火了！在一个狼吃羊的 AI 智障游戏中，狼发现自己吃不到羊，直接选择了「自杀」。然而，狼选择撞石的原因竟是「自杀分数高」！

智障 AI 狼最近火了！

在一个狼吃羊的 AI 游戏中，狼发现自己吃不到羊，而选择了「自杀」。

![](https://mmbiz.qpic.cn/mmbiz_gif/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDnXApo3zRKFIcjIdqEBZtnC9zn880wXs4ZuH5SWoyClLJRzkMyEZZWw/640?wx_fmt=gif)

那么，狼为啥会选择直接撞死呢？

近日，微博上一位网友 @二雨 TR 最近发文称，听我老师给我讲他搞游戏 ai 的事情笑死我了。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GD0auGvpAuRbo8NBS8lribvqSBHCictiakLIxB76U7GicjGficRdyUqOqWvrA/640?wx_fmt=png)

在他发布的这三张聊天记录截屏中，具体介绍了这个狼抓羊的游戏机制。

![](https://mmbiz.qpic.cn/mmbiz_jpg/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDpr2fJdpfqctbG5MsVVb50icaAs0B9JticXg4ysmbusxtPKWx4zib8yt5w/640?wx_fmt=jpeg)

从截图中可以看出，狼选择撞石的原因竟是，「自杀分数高！」

在这个项目中，研究人员给设定了狼吃羊游戏的基本原则是，狼在 20 秒内得分越高越好，而羊在 20 秒内存活时间越长得分越高。

开局两只狼，还有六只羊，地图上红色带 × 的字符就是狼和羊随机出现的可能位置。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDgD0cC8LzNcbLt27ibaKXtUibTAW125FuQ62UILkRWDgibWjHN3pIUovEQ/640?wx_fmt=png)

狼和羊前面有 6 根射线，是用来感知范围。当这 6 根线和障碍物以及地图边界碰撞，就会返回一个坐标。

那根坐标白线便是狼和离它最近羊的连接，这样狼就可以每次优先吃掉最近的那只羊。

在研究人员开始训练的最初阶段，先固定了羊的位置，让狼去学习抓羊。

在狼学会抓羊后，羊也以随机的位置出现在游戏中。

狼抓到羊，奖励 10 分

狼撞到障碍物，扣 1 分

为了节省狼抓羊的时间，每秒钟狼都会受到 0.1 的惩罚

其中，羊撞到石头不会死，只要存活时间长，羊就能得到高分。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GD9DNkS3066Dsv8oricXZibohuRH6UIG79eaYdhYnfyrR3LAgehJjiaHLXQ/640?wx_fmt=png)

如果这两只狼想要在 20 秒以内得到高分，需要狼吃到羊的数量越多越好，吃羊所用时间越短越好。

在研究人员进行了 20W 次的训练，竟发现狼抓羊的效果越来越差。

大多数情况下狼基本吃不到羊，而且在抓羊的过程中浪费的时间也被扣分，干脆就选择撞死了！

该项目的一位研究人员 @Sdust 星尘研表示，「之所以会自杀, 是因为狼在前几万次的训练中发现一头撞死只扣 - 1.1 分 (-1 + -0.1)。

往羊那边走两步撞死扣 - 1.1 到 - 2.4 分。

偶尔一次能吃到，虽然正分，但是不值得」。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDxVrmnMibHun4ltias2kZxgpz5fiaR6QJHfNOStEIkOTqyGcFT7VhH6ialA/640?wx_fmt=png)

这只蠢狼已经在微博、知乎、豆瓣等各大平台上火出了圈。

网友们从狼抓羊的身上看到了自己。

那只狼不就是现在的我么！

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDm450NrQe3cICfVvMC3Ewn3TSm5xSQzXYgps8AC3HEQ268oYKcJFHkQ/640?wx_fmt=png)

狼就是打工人… 每秒扣的是青春和时间，羊是永远达不到的「升职、加薪、迎娶白富美、走上人生巅峰」，撞石头就是躺平摸鱼…

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDLT9pSstqdCpoIIqClXQSEQXmAXfkkhbfaKmN899EiaP7X3ssPdzb09A/640?wx_fmt=png)

还有网友表示，「AI 训练告诉你，为什么现在的年轻人都不愿意努力了」。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDfCLlvUeA5wtcAUSVhWBMeuJrIIFR2Jpuq4SM95ibIicdtQ1hFoshQtJw/640?wx_fmt=png)

有网友对这一项目的奖励机制设置是否合理提出了质疑。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDVibiazlicLaxUyvMjI7LHMibsLJDKVQ7M3FcibdyrY2vdV8yJgibcg8TIV6w/640?wx_fmt=png)

还有网友认为，单步惩罚太大，而撞障碍物的惩罚太小，应该把奖励函数设置为，撞到障碍物的惩罚无穷大，那么狼就知道了撞石的代价，就不会轻易选择自杀了。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDpHQNXGc86FuJ3YsvIxYjnvVDP5bQNluuUI4r4ZuibLNYvicpj8BtnxoA/640?wx_fmt=png)

所以，狼选择自杀的部分原因也是奖励机制设置不合理而导致的。

星尘研在 B 站中的视频表示，狼自杀的错误是很多因素共同影响产生的，最主要的原因是迭代次数太少，20W 次完全不够学。后面提高到 100W 次起步，效果直线上升。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDweNM5qPJJKO5OuPDN8zibicD3icicubxsDic5IIIYibR33tS0Slt4aXb4uxw/640?wx_fmt=png)

训练次数从最初 5W 次一轮，迭代了 13 代。到后来改成 200W 一轮，迭代了 5 代，狼抓羊的训练效果明显提升。

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDITBERXrGxh3iaHXAkYhdjSIdRe7cUcQWSGgq3ORDYWkaZBB9YiaDBfdQ/640?wx_fmt=png)

在训练了 300 万次后，狼终于可以成功地吃到羊。

![](https://mmbiz.qpic.cn/mmbiz_gif/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDwIJF1M3N8ZPk8GAo2icVgibgyIIXpIuomcxBefGlfvQuOnVhIxj9QJDw/640?wx_fmt=gif)

但是，游戏还是存在一定的缺陷，两只狼还是会偶尔撞石而死。

![](https://mmbiz.qpic.cn/mmbiz_gif/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDK55n0Hnqdgyy9vmAeGmk1MYQqcAnP2J9p6qvBbCCgT2H5jibDCuGKCg/640?wx_fmt=gif)

狼终于学会了抓羊\~~

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1xy6UVdHXAg1u01bo1ib4GDQ19OHh19t0a9ic52oOIvOiapI1SkhnohPdWffBS4QCNTcBZvTwjknP1A/640?wx_fmt=png)

参考资料：

[https://m.weibo.cn/6611961566/4613651452134398](https://m.weibo.cn/6611961566/4613651452134398) [https://m.weibo.cn/6611961566/4613930355525879](https://m.weibo.cn/6611961566/4613930355525879)

[https://www.bilibili.com/video/BV16X4y1V7Yu?p=1](https://www.bilibili.com/video/BV16X4y1V7Yu?p=1)

![](https://mmbiz.qpic.cn/mmbiz_png/UicQ7HgWiaUb1yDzUTuNqKX1Eh4DaeyE9zZyc2e79EmWgXJ5956VYaJbdBFRibWaThASUia4y5CGRjomnxu3DIOvmg/640?wx_fmt=png) 
 [https://mp.weixin.qq.com/s/kpqakpeKru7dpkE0f8pySA](https://mp.weixin.qq.com/s/kpqakpeKru7dpkE0f8pySA)
