jQuery.render plugin is a jQuery templates rendering plugin.

// TODO: complete this file


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