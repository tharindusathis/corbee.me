# meant [![Build Status](https://travis-ci.org/watilde/meant.png?branch=master)](https://travis-ci.org/watilde/meant)

Like the `Did you mean?` in git for npm

## API
### meant(item, list)
+ item {String} A key for finding an approximate value
+ list {Array} A list for comparing with the item

```js
const meant = require('meant')
const result = meant('foa', ['foo', 'bar', 'baz'])
// => [ 'foo' ]
```

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install meant --save
```


## Tests

```sh
npm install
npm test
```
```

> meant@1.0.0 test /Users/watilde/Development/meant
> standard && tap test.js
TAP version 13
# Subtest: test.js
    # Subtest: test vs ['tast', 'tbst', 'tcst', 'foo']
        ok 1 - list has tast
        ok 2 - list has tbst
        ok 3 - list has tcst
        ok 4 - list doesn't have foo
        1..4
    ok 1 - test vs ['tast', 'tbst', 'tcst', 'foo'] # time=11.816ms
    1..1
    # time=44.006ms
ok 1 - test.js # time=249.154ms
1..1
# time=267.371ms

```

## Dependencies

None

## Dev Dependencies

- [standard](https://github.com/feross/standard): JavaScript Standard Style
- [standard-version](https://github.com/conventional-changelog/standard-version): replacement for `npm version` with automatic CHANGELOG generation
- [tap](https://github.com/tapjs/node-tap): A Test-Anything-Protocol library


## License

MIT

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_