# @erboladaiorg/molestias-nulla-dolor <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

> Returns true if a value has the characteristics of a valid JavaScript accessor descriptor.

## Examples

```js
const isAccessorDescriptor = require('@erboladaiorg/molestias-nulla-dolor');
const assert = require('assert');

const obj = {
	get foo() {},
	bar: { get: function() {} }
};

assert.equal(true, isAccessorDescriptor(obj, 'foo'));
assert.equal(false, isAccessorDescriptor(obj, 'bar'));

// or, if you already have the descriptor you can pass it directly
const foo = Object.getOwnPropertyDescriptor(obj, 'foo');
assert.equal(true, isAccessorDescriptor(foo));

const bar = Object.getOwnPropertyDescriptor(obj, 'bar');
assert.equal(false, isAccessorDescriptor(bar));
```

### Related projects

You might also be interested in these projects:

* [is-data-descriptor](https://www.npmjs.com/package/is-data-descriptor): Returns true if a value has the characteristics of a valid JavaScript data descriptor.
* [is-descriptor](https://www.npmjs.com/package/is-descriptor): Returns true if a value has the characteristics of a valid JavaScript descriptor. Works for… [more](https://github.com/inspect-js/is-descriptor)
* [is-object](https://www.npmjs.com/package/is-object): Returns true if the value is an object and not an array or null.

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@erboladaiorg/molestias-nulla-dolor
[npm-version-svg]: https://versionbadg.es/inspect-js/@erboladaiorg/molestias-nulla-dolor.svg
[deps-svg]: https://david-dm.org/inspect-js/@erboladaiorg/molestias-nulla-dolor.svg
[deps-url]: https://david-dm.org/inspect-js/@erboladaiorg/molestias-nulla-dolor
[dev-deps-svg]: https://david-dm.org/inspect-js/@erboladaiorg/molestias-nulla-dolor/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@erboladaiorg/molestias-nulla-dolor#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@erboladaiorg/molestias-nulla-dolor.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@erboladaiorg/molestias-nulla-dolor.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@erboladaiorg/molestias-nulla-dolor.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@erboladaiorg/molestias-nulla-dolor
[codecov-image]: https://codecov.io/gh/inspect-js/@erboladaiorg/molestias-nulla-dolor/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@erboladaiorg/molestias-nulla-dolor/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@erboladaiorg/molestias-nulla-dolor
[actions-url]: https://github.com/erboladaiorg/molestias-nulla-dolor/actions
