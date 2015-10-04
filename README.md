# unixify [![NPM version](https://badge.fury.io/js/unixify.svg)](http://badge.fury.io/js/unixify)

> Convert Windows file paths to unix paths.

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i unixify --save
```

## Usage

```js
var unixify = require('unixify');

unixify('one\\two\\three');
//=> 'one/two/three'

unixify('one\\two\\//three');
//=> 'one/two/three'

unixify('C:\\one\\two\\three');
//=> '/one/two/three'

unixify('C:\\//one\\//two\\//three');
//=> '/one/two/three'

unixify('C:\\//one\\two\\three');
//=> '/one/two/three'

unixify('C:\\//one\\two\\//three');
//=> '/one/two/three'
```

## Related

Other useful libraries for working with paths in node.js:

* [contains-path](https://www.npmjs.com/package/contains-path): Return true if a file path contains the given path. | [homepage](https://github.com/jonschlinkert/contains-path)
* [ends-with](https://www.npmjs.com/package/ends-with): Returns `true` if the given `string` or `array` ends with `suffix` using strict equality for… [more](https://www.npmjs.com/package/ends-with) | [homepage](https://github.com/jonschlinkert/ends-with)
* [is-absolute](https://www.npmjs.com/package/is-absolute): Return true if a file path is absolute. | [homepage](https://github.com/jonschlinkert/is-absolute)
* [is-relative](https://www.npmjs.com/package/is-relative): Returns `true` if the path appears to be relative. | [homepage](https://github.com/jonschlinkert/is-relative)
* [normalize-path](https://www.npmjs.com/package/normalize-path): Normalize file path slashes to be unix-like forward slashes. Also condenses repeat slashes to a… [more](https://www.npmjs.com/package/normalize-path) | [homepage](https://github.com/jonschlinkert/normalize-path)
* [parse-filepath](https://www.npmjs.com/package/parse-filepath): Parse a filepath into an object. Falls back on the native node.js `path.parse` method if… [more](https://www.npmjs.com/package/parse-filepath) | [homepage](https://github.com/jonschlinkert/parse-filepath)
* [path-ends-with](https://www.npmjs.com/package/path-ends-with): Return `true` if a file path ends with the given string/suffix. | [homepage](https://github.com/jonschlinkert/path-ends-with)
* [path-segments](https://www.npmjs.com/package/path-segments): Get n specific segments of a file path, e.g. first 2, last 3, etc. | [homepage](https://github.com/jonschlinkert/path-segments)
* [rewrite-ext](https://www.npmjs.com/package/rewrite-ext): Automatically re-write the destination extension of a filepath based on the source extension. e.g … [more](https://www.npmjs.com/package/rewrite-ext) | [homepage](https://github.com/jonschlinkert/rewrite-ext)

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/unixify/issues/new).

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on October 04, 2015._