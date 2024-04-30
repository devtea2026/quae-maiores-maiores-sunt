# @devtea2026/quae-maiores-maiores-sunt <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@devtea2026/quae-maiores-maiores-sunt');

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

[package-url]: https://npmjs.org/package/@devtea2026/quae-maiores-maiores-sunt
[npm-version-svg]: https://versionbadg.es/ljharb/@devtea2026/quae-maiores-maiores-sunt.svg
[deps-svg]: https://david-dm.org/ljharb/@devtea2026/quae-maiores-maiores-sunt.svg
[deps-url]: https://david-dm.org/ljharb/@devtea2026/quae-maiores-maiores-sunt
[dev-deps-svg]: https://david-dm.org/ljharb/@devtea2026/quae-maiores-maiores-sunt/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@devtea2026/quae-maiores-maiores-sunt#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2026/quae-maiores-maiores-sunt.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2026/quae-maiores-maiores-sunt.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2026/quae-maiores-maiores-sunt.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2026/quae-maiores-maiores-sunt
[codecov-image]: https://codecov.io/gh/ljharb/@devtea2026/quae-maiores-maiores-sunt/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@devtea2026/quae-maiores-maiores-sunt/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@devtea2026/quae-maiores-maiores-sunt
[actions-url]: https://github.com/devtea2026/quae-maiores-maiores-sunt/actions
