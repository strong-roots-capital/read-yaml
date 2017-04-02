# read-yaml [![NPM version](https://img.shields.io/npm/v/read-yaml.svg?style=flat)](https://www.npmjs.com/package/read-yaml) [![NPM monthly downloads](https://img.shields.io/npm/dm/read-yaml.svg?style=flat)](https://npmjs.org/package/read-yaml)  [![NPM total downloads](https://img.shields.io/npm/dt/read-yaml.svg?style=flat)](https://npmjs.org/package/read-yaml) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/read-yaml.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/read-yaml)

> Very thin wrapper around js-yaml for directly reading in YAML files.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save read-yaml
```

## API

### [readYaml](index.js#L29)

Read yaml file asynchronously and parse content as JSON.

**Params**

* `filepath` **{String}**: Path of the file to read.
* `options` **{Object|String}**: to pass to [js-yaml](https://github.com/nodeca/js-yaml)
* `cb` **{Function}**: Callback function `

**Example**

```js
var readYaml = require('read-yaml');
readYaml('config.yml', function(err, data) {
  if (err) throw err;
  console.log(data);
});
```

### [.sync](index.js#L69)

Read yaml file synchronously and parse content as JSON.

**Params**

* `filepath` **{String}**: Path of the file to read.
* `options` **{Object|String}**: to pass to [js-yaml](https://github.com/nodeca/js-yaml).
* `returns` **{Object}**: JSON

**Example**

```js
var read = require('read-yaml');
var config = read.sync('config.yml');
```

## About

### Related projects

* [copy](https://www.npmjs.com/package/copy): Copy files or directories using globs. | [homepage](https://github.com/jonschlinkert/copy "Copy files or directories using globs.")
* [read-data](https://www.npmjs.com/package/read-data): Read JSON or YAML files. | [homepage](https://github.com/jonschlinkert/read-data "Read JSON or YAML files.")
* [write](https://www.npmjs.com/package/write): Write files to disk, creating intermediate directories if they don't exist. | [homepage](https://github.com/jonschlinkert/write "Write files to disk, creating intermediate directories if they don't exist.")

### Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

### Contributors

| **Commits** | **Contributor** | 
| --- | --- |
| 15 | [shinnn](https://github.com/shinnn) |
| 10 | [jonschlinkert](https://github.com/jonschlinkert) |

### Building docs

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

### Running tests

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

### Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.4.3, on April 02, 2017._