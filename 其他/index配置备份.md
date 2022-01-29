```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>知识库</title>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
  <meta name="description" content="Description">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/buble.css">
  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar.min.css" />
  <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar-folder.min.css" />
</head>
<style type="text/css">
.content {
  overflow: auto;
}
</style>
<body>
  <div id="app"></div>
  <script>
    window.$docsify = {
      loadNavbar: true,
      loadSidebar: true,
      subMaxLevel: 3,
      name: '风沙星辰',
		search: 'auto',

      relativePath: true,
      auto2top: true,
      
		count:{
		countable:true,
		fontsize:'0.9em',
		color:'rgb(90,90,90)',
		language:'chinese'
		},
		formatUpdated: '{MM}/{DD} {HH}:{mm}',
		formatUpdated: function(time) {
		// ...
		return time;
		},


    };
  </script>
	<!-- Docsify v4 -->
	<script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
	
	<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/zoom-image.min.js"></script>

	<script src="//unpkg.com/docsify-count/dist/countable.js"></script>
	
	<!-- sidebarfold -->
	<script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>

	<!-- search -->
	<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>
	<script src="//polyfill.io/v3/polyfill.min.js?features=String.prototype.normalize"></script>
</body>
</html>

```

