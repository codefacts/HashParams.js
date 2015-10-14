# HashParams.js
JavaScript hash manipulation library.
Hash.js - URL Hash Manipulation
Hash.js is a 0.5 KB script that lets you in a super simple way manipulate everything behind # in urls. Tested in latest Chrome, Safari, Firefox and IE7,8,9.

See example page at jonnystromberg.com/hash-js or see it in action at PNGTextures.com.

Btw, follow me (@javve) at Twitter and checkout my other project List.js

Notice: The main focus of Hash.js is simplicity. This is no tool for your super-ajax-native-feeling-app-with-google-bot-support. If that's your usage situation, use the awesome History.js.

Usage

Just include hash.min.js or hash.js at your site and then a hash object will become available.

<script src="hash.min.js"></script>

<script>
    hash.add({foo: "bar" });                // Url becomes http://url.com#foo=bar
</scrtip>
Methods

hash.add(params)
Add parameter to hash

hash.add({ foo: "bar" });               // http://url.com#foo=bar
hash.add({ car: "dar", sar: "par" });   // http://url.com#foo=bar&car=dar&sar=par
hash.get(param) or hash.get()
Returns value of paramter in hash. If param is undefined then all values are returned.

var fooValue = hash.get('foo');         // fooValue == "bar"
var allValues = hash.get();             // allValues == { foo: "bar", car: "dar", sar: "par"}
hash.remove(param)
Removes the value with name param.

hash.remove('foo');                     // http://url.com#car=dar&sar=par
hash.clear()
Clears entire hash.

hash.clear();                           // http://url.com#
License

DON'T BE A DICK PUBLIC LICENSE

Version 1, December 2009

Copyright (C) 2011
Jonny Strömberg @javve

Everyone is permitted to copy and distribute verbatim or modified copies of this license document, and changing it is allowed as long as the name is changed.
