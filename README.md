[![Build Status](https://travis-ci.org/pelevesque/supersubstr.svg?branch=master)](https://travis-ci.org/pelevesque/supersubstr)
[![Coverage Status](https://coveralls.io/repos/github/pelevesque/supersubstr/badge.svg?branch=master)](https://coveralls.io/github/pelevesque/supersubstr?branch=master)
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

# supersubstr

Like Javascript's substr, but with wrapping and reversed substrings.

## Node Repository

https://www.npmjs.com/package/@pelevesque/supersubstr

## Installation

`npm install @pelevesque/supersubstr`

## Tests

### Standard Style & Unit Tests

`npm test`

### Unit Tests & Coverage

`npm run cover`

## Usage

### parameters

```js
str     (required)
options (optional) default = { startIndex = 0, length, reverse = false }
```

### examples

```js
const supersubstr = require('@pelevesque/supersubstr')
```

```js
const str = '12345'
const result = supersubstr(str, { startIndex: 1 })
// result === '2345'
```

```js
const str = '12345'
const result = supersubstr(str, { startIndex: 2, length: 10, reverse: true })
// result === '3215432154'
```
