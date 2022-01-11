![RealToNumber][real-to-number-logo]
# 🔢 RealToNumber

Convert your real(pt-BR) string to float number ou other types.

## Installation

This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry][real-to-number-logo-npm].

Use npm:
```bash
$ npm install realtonumber
```

Use yarn:
```bash
$ yarn add realtonumber
```


## Features
- realToFloat - Convert real to float
- realToInt - Convert real to int


## Examples
1. Convert string to float.
```javascript
const {realToFloat} = require('realtonumber');

let number = realToFloat('R$ 12.345,67');
// > 12345.67

let number = realToFloat('R$ 12.345,6789', {
    decimal: 3
});
// > 12345.678

```
Options:
- decimal: number > Number of decimal cases in this number.


2. Convert string to int.
```javascript
const {realToInt} = require('realtonumber');

let number = realToInt('R$ 12.345,67');
// > 12346

let number = realToInt('R$ 12.345,6789', {
    useDecimal: true
});
// > 1234568

```
Options:
- useDecimal: boolean > When you active this option, your number remove ',' and use 2 number after.


****
This project is under the MIT license. See the [LICENSE][license-link] file for more details

<!-- Markdown link & img's -->
[license-link]: /LICENSE
[real-to-number-logo]: https://i.imgur.com/eb9Cxqe.png
[real-to-number-logo-npm]: https://www.npmjs.com/package/cowmmand
