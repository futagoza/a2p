[![Build status](https://api.travis-ci.org/futagoza/a2p.svg?branch=master)](https://travis-ci.org/futagoza/a2p)
[![npm version](https://img.shields.io/npm/v/a2p.svg)](https://www.npmjs.com/package/a2p)
[![devDependencies](https://img.shields.io/david/dev/futagoza/a2p.svg)](https://david-dm.org/futagoza/a2p#info=devDependencies)
[![License](https://img.shields.io/badge/license-mit-blue.svg)](https://opensource.org/licenses/MIT)

> ES2017 async and await, as Promise's

## features

A2P is a library that provides various methods that implement:

* `execute`, a function executer, faster then `Function.prototype.call`
* `attempt`, a wrapper for `try {} catch ( e ) {}`
* `Promise`, a small and fast ES2015 Promise implmentaion
* `Async`, a defered Promise
* `Await`, a smart-wrapper to always return a Promise

## dist outline

* ES5 AMD: `dist/a2p-es5.amd.js`
* ES5 CommonJS: `dist/a2p-es5.commonjs.js`
* ES5 UMD: `dist/a2p-es5.umd.js`
* ES6 AMD: `dist/a2p-es6.amd.js`
* ES6 CommonJS: `dist/a2p-es6.commonjs.js`
* ES6 Module: `dist/a2p-es6.module.js`
* ES6 UMD: `dist/a2p-es6.umd.js`

## installation

### npm

```bash
$ npm install a2p --save
```

### bower

```bash
$ bower install a2p=futagoza/a2p --save
```

## usage

### node.js

```js
// Automatically require's `a2p/dist/a2p-es5.commonjs.js` or `a2p/dist/a2p-es6.commonjs.js`.
const a2p = require( "a2p" );
```

### browser (es5, global/amd)

```html
<script src="bower_components/a2p/dist/a2p-es5.umd.js"></script>
```

```js
// global
var a2p = window.a2p;

// amd
define( function( require ) {

    var a2p = require( "a2p" );

    // ...

} );
```

### browser (es5, amd only)

```js
define( [ "/bower_components/a2p/dist/a2p-es5.amd.js" ], function( a2p ) {

    // ...

} );
```

## license

Copyright © 2017 Futago-za Ryuu, [https://github.com/futagoza](https://github.com/futagoza)<br />
Released under the MIT License, [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)
