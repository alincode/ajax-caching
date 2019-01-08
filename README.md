# AJAX caching

![GitHub package version](https://img.shields.io/github/package-json/v/alincode/ajax-caching.svg)
![node version](https://img.shields.io/node/v/ajax-caching.svg)
![npm downloads](https://img.shields.io/npm/dt/ajax-caching.svg)
[![Dependency Status](https://img.shields.io/david/alincode/ajax-caching.svg?style=flat)](https://david-dm.org/alincode/ajax-caching)

### Feature

* It could help you quickly AJAX caching result.

### Install

```sh
npm install ajax-caching
```

### usage

* use cache

```js
const compilerURL = 'https://solc-bin.ethereum.org/bin/soljson-v0.4.25+commit.59dbf8f1.js';
const opts = { url: compilerURL, caching: true };
let source = await promiseAjax(opts);
```

* don't use cache

```js
const compilerURL = 'https://solc-bin.ethereum.org/bin/soljson-v0.4.25+commit.59dbf8f1.js';
const opts = { url: compilerURL, caching: false };
let source = await promiseAjax(opts);
```

* simple to use

```js
const compilerURL = 'https://solc-bin.ethereum.org/bin/soljson-v0.4.25+commit.59dbf8f1.js';
let source = await promiseAjax(compilerURL);
```

## License
MIT © [alincode](https://github.com/alincode/ajax-caching)