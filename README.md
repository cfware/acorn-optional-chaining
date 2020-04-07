# Optional Chaining Support for Acorn

[![NPM version](https://img.shields.io/npm/v/acorn-optional-chaining.svg)](https://www.npmjs.org/package/acorn-optional-chaining)

This is a plugin for [Acorn](https://github.com/acornjs/acorn) - a tiny, fast JavaScript parser, written completely in JavaScript.

## Purpose of this fork

This fork exists to enable compatibility with rollup 2.x.  This will be deprecated and archived once
compatibility is merged [upstream](https://github.com/rockon999/acorn-optional-chaining).

## Usage

This module provides a plugin which extends the Acorn `Parser` class to handle optional chaining:

```javascript
import * as acorn from 'acorn';
import optionalChaining from 'acorn-optional-chaining';

acorn.Parser.extend(optionalChaining).parse('a?.b?.c');
```

## License

This plugin is released under an [MIT License](./LICENSE).

It was based off the structure of [`acorn-numeric-separator`](https://github.com/acornjs/acorn-numeric-separator).
