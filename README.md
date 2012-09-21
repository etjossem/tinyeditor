tinyeditor
==========

TinyEditor is a simple JavaScript WYSIWYG editor that is both lightweight (under 9KB) and standalone. It can easily be customized to integrate with any website through CSS and the multitude of parameters. It handles most of the basic formatting needs and has some functionality built in to help keep the rendered markup as clean as possible. The icons are courtesy of famfamfam and have been combined into a sprite so there are only a few HTTP requests for the editor.

Usage:

```
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>TinyEditor - JavaScript WYSIWYG Editor</title>
<link rel="stylesheet" href="tinyeditor.css">
<script src="tiny.editor.packed.js"></script>
</head>
<body>
<textarea id="tinyeditor" style="width: 400px; height: 200px"></textarea>
<script>
var editor = new TINY.editor.edit('editor', {
	id: 'tinyeditor',
	width: 584,
	height: 175,
	cssclass: 'tinyeditor',
	controlclass: 'tinyeditor-control',
	rowclass: 'tinyeditor-header',
	dividerclass: 'tinyeditor-divider',
	controls: ['bold', 'italic', 'underline', 'strikethrough', '|', 'subscript', 'superscript', '|',
		'orderedlist', 'unorderedlist', '|', 'outdent', 'indent', '|', 'leftalign',
		'centeralign', 'rightalign', 'blockjustify', '|', 'unformat', '|', 'undo', 'redo', 'n',
		'font', 'size', 'style', '|', 'image', 'hr', 'link', 'unlink', '|', 'print'],
	footer: true,
	fonts: ['Verdana','Arial','Georgia','Trebuchet MS'],
	xhtml: true,
	cssfile: 'custom.css',
	bodyid: 'editor',
	footerclass: 'tinyeditor-footer',
	toggle: {text: 'source', activetext: 'wysiwyg', cssclass: 'toggle'},
	resize: {cssclass: 'resize'}
});
</script>
</body>
</html>
```
