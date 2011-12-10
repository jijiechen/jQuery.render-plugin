jQuery.render plugin is a jQuery templates rendering plugin.

Them complete introduction of this plugin is available at http://blog.ciznx.com/projects/jQuery.render.doc-cn.html （currently in Chinese）
jQuery.render 插件的完整文档，请访问 blog.ciznx.com/projects/jQuery.render.doc-cn.html（中文）


Usage:


<ul id="panel"></ul>

<script type="text/template" id="tmpl">

	<li>Name:<?= name ?></li>
	<li>Age:<?= age ?></li>
	<li>Gender:<?=(ismale ?  "male" : "female") ?></li>
	
</script>


<script type="text/javascript">
	
	var data = {
		age: 28,
		name: 'ciznx chan',
		ismale: true
	};
	
	$("#panel").render(data, $("#tmpl"));
	
</script>