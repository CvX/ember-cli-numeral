# ember-cli-numeral
[![Build Status](https://travis-ci.org/josemarluedke/ember-cli-numeral.svg?branch=master)](https://travis-ci.org/josemarluedke/ember-cli-numeral)
[![Ember Observer Score](https://emberobserver.com/badges/ember-cli-numeral.svg)](https://emberobserver.com/addons/ember-cli-numeral)
[![NPM Version](https://img.shields.io/npm/v/ember-cli-numeral.svg?style=flat-square)](https://www.npmjs.com/package/ember-cli-numeral)
[![Ember badge](https://embadge.io/v1/badge.svg?start=1.13.0)](https://embadge.io/)

ES6 accessible module for Numeral.js within your Ember applications.

## Install

```bash
ember install ember-cli-numeral
```

## Usage

```javascript
import numeral from 'numeral';

let string = numeral(1000).format('0,0');
// '1,000'
```

See the [Numeral.js docs](http://numeraljs.com/) for general usage.

## Including Numeral.js locales

To include all the Numeral.js locales definitions, you need to add the
following configuration to your `ember-cli-build.js`.

```javascript
var app = new EmberApp(defaults, {
  numeral: {
    includeLocales: true
  }
});
```

Then import locales to register them:

```javascript
import 'numeral-locales';
```

The default configuration is `false`. So locales will not be loaded by default.

## FastBoot compatibility

This addon is compatible with [FastBoot](http://ember-fastboot.com/) out of the box.

## License

`ember-cli-numeral` shims is MIT Licensed.
