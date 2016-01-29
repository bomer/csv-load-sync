# csv-load-sync

Sync loading routine for a small comma-separated values file (.csv). Returns an array of objects, takes property names from
the first line. Assumes everything is a string in quotes.

[![Package info][nodei.co]](https://npmjs.org/package/csv-load-sync)

[![Build status][ci-image]][ci-status]
[![dependencies][dependencies-image]][dependencies-url]
[![semantic-release][semantic-image] ][semantic-url]

## Install

Requires nodejs

    npm install csv-load-sync

## Inputs

Example CSV file with two records

    "deviceId","description"
    "1","iPhone 4"
    "2","iPhone 4S"

Example CSV file with three records

    "id","firstName","lastName","country","lastLogin"
    "1","John","Smith","US","2013-08-04 23:57:38"
    "2","Greg","Smith","US","2013-07-12 13:27:18"
    "3","Harold","Smith","GB","2013-07-16 21:17:28"

## Example

```js
var loader = require('csv-load-sync');
var csv = loader('path/to/file.csv');
// csv is an Array of objects
```

### Fine print

Author: Gleb Bahmutov &copy; 2015

* [@bahmutov](https://twitter.com/bahmutov)
* [glebbahmutov.com](http://glebbahmutov.com)
* [blog](http://glebbahmutov.com/blog/)

License: MIT - do anything with the code, but don't blame me if it does not work.

Spread the word: tweet, star on github, etc.

[ci-image]: https://secure.travis-ci.org/bahmutov/csv-load-sync.png?branch=master
[ci-status]: http://travis-ci.org/#!/bahmutov/csv-load-sync
[nodei.co]: https://nodei.co/npm/csv-load-sync.png?downloads=true
[dependencies-image]: https://david-dm.org/bahmutov/csv-load-sync.png
[dependencies-url]: https://david-dm.org/bahmutov/csv-load-sync
[semantic-image]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-url]: https://github.com/semantic-release/semantic-release
