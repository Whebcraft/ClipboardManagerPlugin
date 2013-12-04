##Phonegap Android plugin for interacting with Android ClipbaordManager##

This version of the plugin is for Phonegap versions >= 3.0.0

use cordova cli to add this plugin:
```bash
cordova plugin add https://github.com/gitawego/ClipboardManagerPlugin.git
```

`navigator.clipboardManager.copy(str, success, fail)` that copies the given string into the clipboard
`navigator.clipboardManager.paste(success, fail)` that returns the text from the clipboard

`success` and `fail` are callback functions. 

An example for copy:
```js
	navigator.clipboardManager.copy(
		"the text to copy",
		function(r){alert("copy is successful")},
		function(e){alert(e)}
	);
```

An example for paste:
```js
	navigator.clipboardManager.paste(
		function(r){alert("The text in the clipboard is " + r)},
		function(e){alert(e)}
	);
```
