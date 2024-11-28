# @kizahasi/option

![GitHub](https://img.shields.io/github/license/kizahasi/option) [![npm version](https://img.shields.io/npm/v/@kizahasi/option.svg?style=flat)](https://www.npmjs.com/package/@kizahasi/option) ![minified size](https://img.shields.io/bundlephobia/min/@kizahasi/option) [![CI](https://github.com/kizahasi/option/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kizahasi/option/actions/workflows/ci.yml) [![publish](https://github.com/kizahasi/option/actions/workflows/publish.yml/badge.svg?branch=release)](https://github.com/kizahasi/option/actions/workflows/publish.yml)

Represents a value which is either Some or None.

## Installation

Run `npm install @kizahasi/option` or `yarn add @kizahasi/option`

## Usage

```typescript
import { Option } from '@kizahasi/option';

const someObj = Option.some(1);
if (someObj.isNone) {
    console.log('none'); // This cannot happen
} else {
    console.log(someObj.value); // output: 1
}

const noneObj = Option.none();
if (noneObj.isNone) {
    console.log('none'); // output: none
} else {
    console.log(noneObj.value); // This cannot happen
}
```

## License

MIT or CC0-1.0
