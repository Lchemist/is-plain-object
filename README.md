# is-plain-object [![NPM version](https://img.shields.io/npm/v/is-plain-object.svg?style=flat)](https://www.npmjs.com/package/is-plain-object) [![NPM monthly downloads](https://img.shields.io/npm/dm/is-plain-object.svg?style=flat)](https://npmjs.org/package/is-plain-object) [![NPM total downloads](https://img.shields.io/npm/dt/is-plain-object.svg?style=flat)](https://npmjs.org/package/is-plain-object) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/is-plain-object.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/is-plain-object)

> Returns true if an object was created by the `Object` constructor, or Object.create(null).

Please consider following this project's author, [Jon Schlinkert](https://github.com/jonschlinkert), and consider starring the project to show your :heart: and support.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save is-plain-object
```

Use [isobject](https://github.com/jonschlinkert/isobject) if you only want to check if the value is an object and not an array or null.

## Usage

with es modules
```js
import { isPlainObject } from 'is-plain-object';
```

or with commonjs
```js
const { isPlainObject } = require('is-plain-object');
```

**true** when created by the `Object` constructor, or Object.create(null).

```js
isPlainObject(Object.create({}));
//=> true
isPlainObject(Object.create(null));
//=> true
isPlainObject(Object.create(Object.prototype));
//=> true
isPlainObject({foo: 'bar'});
//=> true
isPlainObject({});
//=> true
isPlainObject(null);
//=> true
```

**false** when not created by the `Object` constructor.

```js
isPlainObject(1);
//=> false
isPlainObject(['foo', 'bar']);
//=> false
isPlainObject([]);
//=> false
isPlainObject(new Foo);
//=> false
```

## About

<details>
<summary><strong>Contributing</strong></summary>

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

</details>

<details>
<summary><strong>Running Tests</strong></summary>

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

</details>

<details>
<summary><strong>Building docs</strong></summary>

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

</details>

### Related projects

You might also be interested in these projects:

* [is-number](https://www.npmjs.com/package/is-number): Returns true if a number or string value is a finite number. Useful for regex… [more](https://github.com/jonschlinkert/is-number) | [homepage](https://github.com/jonschlinkert/is-number "Returns true if a number or string value is a finite number. Useful for regex matches, parsing, user input, etc.")
* [isobject](https://www.npmjs.com/package/isobject): Returns true if the value is an object and not an array or null. | [homepage](https://github.com/jonschlinkert/isobject "Returns true if the value is an object and not an array or null.")
* [kind-of](https://www.npmjs.com/package/kind-of): Get the native type of a value. | [homepage](https://github.com/jonschlinkert/kind-of "Get the native type of a value.")

### Contributors

| **Commits** | **Contributor** |  
| --- | --- |  
| 19 | [jonschlinkert](https://github.com/jonschlinkert) |  
| 6  | [TrySound](https://github.com/TrySound) |  
| 6  | [stevenvachon](https://github.com/stevenvachon) |  
| 3  | [onokumus](https://github.com/onokumus) |  
| 1  | [wtgtybhertgeghgtwtg](https://github.com/wtgtybhertgeghgtwtg) |  

### Author

**Jon Schlinkert**

* [GitHub Profile](https://github.com/jonschlinkert)
* [Twitter Profile](https://twitter.com/jonschlinkert)
* [LinkedIn Profile](https://linkedin.com/in/jonschlinkert)

### License

Copyright © 2019, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.8.0, on April 28, 2019._
