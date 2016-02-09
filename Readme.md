
# reduce

[![Build status][travis-image]][travis-url]
[![Git tag][git-image]][git-url]
[![NPM version][npm-image]][npm-url]
[![Code style][standard-image]][standard-url]

Reduce over the elements of a container

## Installation

    $ npm install @f/reduce

## Usage

```js
var reduce = require('@f/reduce')
var fruits = {apples: 2, oranges: 3}
var numFruits = reduce(sum, 0, fruits)

function sum (a, b) {
  return a + b
}
```

## API

### reduce(cb, initialValue, collection)

- `cb` - Callback called for each `collection` item with a accumlator value and the current item.

```js
function cb (accumulator, currentItem, key, colllection) {}
```

- `initialValue` - First value for the accumulator
- `arr` Collection to be reduced

**Returns:** The accumulated value

## License

MIT

[travis-image]: https://img.shields.io/travis/micro-js/reduce.svg?style=flat-square
[travis-url]: https://travis-ci.org/micro-js/reduce
[git-image]: https://img.shields.io/github/tag/micro-js/reduce.svg
[git-url]: https://github.com/micro-js/reduce
[standard-image]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat
[standard-url]: https://github.com/feross/standard
[npm-image]: https://img.shields.io/npm/v/@f/reduce.svg?style=flat-square
[npm-url]: https://npmjs.org/package/@f/reduce
