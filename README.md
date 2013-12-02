Phonegap Cookies Plugin
=======

Phonegap/Cordova plugin that allows you to clear cookies of the webview. Use it for logging out the user, restart analytics session etc.

## Why a plugin?

On Phonegap `document.cookie` is empty, index.html and all other files are loaded with `file://` protocol.
Phonegap manages cookies internally, but doesn't expose any function for clearing them.

## Installation:

### Automatically (CLI / Plugman)

Cookies is compatible with [Cordova Plugman](https://github.com/apache/cordova-plugman) and ready for the [PhoneGap 3.0 CLI](http://docs.phonegap.com/en/3.0.0/guide_cli_index.md.html#The%20Command-line%20Interface_add_features), here's how it works with the CLI:

```
$ phonegap local plugin add https://github.com/bez4pieci/Cookies.git
```

## Usage

```javascript
window.cookies.clear(function() {
	console.log('Cookies cleared!');
});
```
