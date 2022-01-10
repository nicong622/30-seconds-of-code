---
title: generateAlphabet
tags: array,intermediate
firstSeen: 2022-01-10T09:56:05.740Z
lastUpdated: 2022-01-10T10:22:53.971Z
---

Generate an array of alphabet from A to Z.

- Use `Array.from()` to create an array.
- Get the UTF-16 code unit value of every character from the alphabet.
- Use `String.fromCharCode()` to create characters from the code unit above.

```js
const generateAlphabet = () => Array.from({ length: 26 }, (_, i) => String.fromCharCode(i + 'A'.charCodeAt()))
```

```js
console.log(generateAlphabet());

/*
[
  'A', 'B', 'C', 'D', 'E', 'F',
  'G', 'H', 'I', 'J', 'K', 'L',
  'M', 'N', 'O', 'P', 'Q', 'R',
  'S', 'T', 'U', 'V', 'W', 'X',
  'Y', 'Z'
]
*/
```
