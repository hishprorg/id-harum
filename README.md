# @hishprorg/id-harum <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@hishprorg/id-harum');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@hishprorg/id-harum
[npm-version-svg]: https://versionbadg.es/ljharb/@hishprorg/id-harum.svg
[deps-svg]: https://david-dm.org/ljharb/@hishprorg/id-harum.svg
[deps-url]: https://david-dm.org/ljharb/@hishprorg/id-harum
[dev-deps-svg]: https://david-dm.org/ljharb/@hishprorg/id-harum/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@hishprorg/id-harum#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@hishprorg/id-harum.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/id-harum.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/id-harum.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/id-harum
[codecov-image]: https://codecov.io/gh/ljharb/@hishprorg/id-harum/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@hishprorg/id-harum/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@hishprorg/id-harum
[actions-url]: https://github.com/hishprorg/id-harum/actions
