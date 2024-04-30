# @f1stnpm2/praesentium-consectetur-culpa <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@f1stnpm2/praesentium-consectetur-culpa');

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

[package-url]: https://npmjs.org/package/@f1stnpm2/praesentium-consectetur-culpa
[npm-version-svg]: https://versionbadg.es/ljharb/@f1stnpm2/praesentium-consectetur-culpa.svg
[deps-svg]: https://david-dm.org/ljharb/@f1stnpm2/praesentium-consectetur-culpa.svg
[deps-url]: https://david-dm.org/ljharb/@f1stnpm2/praesentium-consectetur-culpa
[dev-deps-svg]: https://david-dm.org/ljharb/@f1stnpm2/praesentium-consectetur-culpa/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@f1stnpm2/praesentium-consectetur-culpa#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@f1stnpm2/praesentium-consectetur-culpa.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@f1stnpm2/praesentium-consectetur-culpa.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@f1stnpm2/praesentium-consectetur-culpa.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@f1stnpm2/praesentium-consectetur-culpa
[codecov-image]: https://codecov.io/gh/ljharb/@f1stnpm2/praesentium-consectetur-culpa/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@f1stnpm2/praesentium-consectetur-culpa/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@f1stnpm2/praesentium-consectetur-culpa
[actions-url]: https://github.com/f1stnpm2/praesentium-consectetur-culpa/actions
