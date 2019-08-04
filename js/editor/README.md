# Sources:

ace.js: Via https://github.com/ajaxorg/ace-builds
theme-twilight.js: Via https://github.com/ajaxorg/ace-builds
mode-processing.js: From the hello.processing.org site, via https://stackoverflow.com/a/25216371

# Simplest Example

```
<script src="ace.js" type="text/javascript" charset="utf-8"></script>
<script src="theme-twilight.js" type="text/javascript" charset="utf-8"></script>
<script src="mode-processing.js" type="text/javascript" charset="utf-8"></script>

<div id="editor">some text</div>


<style>
/* editor must have absolute width/height */
#editor {
    position: absolute;
    width: 500px;
    height: 400px;
}
</style>
<script>
    var editor = ace.edit("editor");
    editor.setTheme("ace/theme/twilight");
    var ProcessingMode = ace.require('ace/mode/processing').Mode;
    editor.session.setMode(new ProcessingMode());
</script>
```
