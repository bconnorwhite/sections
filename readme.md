# sections [![NPM version](https://img.shields.io/npm/v/sections.svg)](https://www.npmjs.com/package/sections) [![Build Status](https://img.shields.io/travis/jonschlinkert/sections.svg)](https://travis-ci.org/jonschlinkert/sections)

> Manipulate sections in a string of markdown.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm i sections --save
```

## Usage

This is meant to be fast and opinionated, and only works with [ATX headings](http://spec.commonmark.org/0.24/#atx-headings).

```js
var sections = require('sections');
```

## API

### [.parse](index.js#L23)

Parses sections in a `string` of markdown and returns an object with two properties:

* `sections`: an array of markdown "sections", delimited by [ATX headings](http://spec.commonmark.org/0.24/#atx-headings),
* `result`: the cumulative result of whatever is returned by the (optional) function that is passed as the second argument.

**Params**

* `string` **{String}**
* `fn` **{Function}**
* `returns` **{Object}**

### [.format](index.js#L63)

Format sections. By default, if no filter function is passed, this:

* filters out empty sections
* fixes whitespace between sections

**Params**

* `str` **{String}**: Markdown string
* `fn` **{Function}**: optional filter function
* `returns` **{String}**

## Related projects

* [gulp-format-md](https://www.npmjs.com/package/gulp-format-md): Gulp plugin for beautifying markdown using pretty-remarkable. | [homepage](https://github.com/jonschlinkert/gulp-format-md)
* [markdown-utils](https://www.npmjs.com/package/markdown-utils): Micro-utils for creating markdown snippets. | [homepage](https://github.com/jonschlinkert/markdown-utils)
* [remarkable](https://www.npmjs.com/package/remarkable): Markdown parser, done right. 100% Commonmark support, extensions, syntax plugins, high speed - all in… [more](https://www.npmjs.com/package/remarkable) | [homepage](https://github.com/jonschlinkert/remarkable)

## Generate docs

Generate readme and API documentation with [verb](https://github.com/verbose/verb):

```sh
$ npm i -d && npm run docs
```

Or, if [verb](https://github.com/verbose/verb) is installed globally:

```sh
$ verb
```

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/sections/issues/new).

## Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2016 [Jon Schlinkert](https://github.com/jonschlinkert)
Released under the [MIT license](https://github.com/jonschlinkert/sections/blob/master/LICENSE).

***

_This file was generated by [verb](https://github.com/verbose/verb), v0.9.0, on February 15, 2016._