ffprobe-static
====


**-->Modified version<--** adding `browser`, as a platform option, for use case when module is bundled using browserify. and added to html using src.The module untimately it returns a file path to the binary. This is tailored for a use case such as that of [autoEdit.io](http://autoEdit.io) where it is an electron app where the front end is in backbone and bundled with browserify, while the backend, is a series of node modules, where the code to run ffprobe ultimatly resides. 

see also[modified ffmpeg-static](https://github.com/pietrop/ffmpeg-static)

---

Static binaries for `ffprobe`. OSX only at the moment, please send a PR if you would like to help with adding support for other platforms.

Based on <https://github.com/eugeneware/ffmpeg-static>.

Binaries are from <http://ffmpeg.zeranoe.com/builds/>

Usage
----

```js
var ffprobe = require('ffprobe-static');
console.log(ffprobe.path);
```

Version Notes
----

Currently supports Mac OS X (64-bit), Linux (32 and 64-bit) and Windows
(32 and 64-bit).

Currently version `3.1` is installed for Mac and Linux, and `3.0.1` for
Windows.

I pulled the versions from the ffmpeg static build pages linked from the
official ffmpeg site. Namely:

* [64 bit Mac OSX](https://evermeet.cx/ffmpeg/)
* [64 bit Linux](http://johnvansickle.com/ffmpeg/)
* [32 bit Linux](http://johnvansickle.com/ffmpeg/)
* [64 bit Windows](http://ffmpeg.zeranoe.com/builds/win64/static/)
* [32 bit Windows](http://ffmpeg.zeranoe.com/builds/win32/static/)

Acknowledgements
----

Special thanks to [eugeneware](https://github.com/eugeneware) for <https://github.com/eugeneware/ffmpeg-static>, which this is based upon.
