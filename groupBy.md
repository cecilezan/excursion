---
Title: '.groupBy()'
Description: 'Groups items by arbitrary key.'
Subjects:
  - 'Web Development'
Tags:
  - 'Methods'
  - 'Objects'
CatalogContent:
  - 'introduction-to-javascript'
  - 'paths/full-stack-engineer-career-path'
---

The **`.groupBy()`** method groups items .

## Syntax

```pseudo
Object.groupBy(array, callback function);
```

The `array` is usually an Array .
The `callback function` is callback function with 2 .

## Example

Creating an object from an array.

```js
const array = [1, 2, 3, 4, 5];

const newObject = Object.groupBy(array, (num, index) => {
  return num % 2 === 0 ? 'even': 'odd';
});
// =>  { odd: [1, 3, 5], even: [2, 4] }

console.log(newObject);
```

The output would be:

```shell
{ '0': 'Los Angeles', '1': 'Toronto', '2': 'Paris' }
```

## Codebyte Example

Following is a runnable example that demonstrates the `.fromEntries()` method.

```codebyte/javascript
const gotty2023 = new Map([
  ["Jerry Seinfeld", "Comedian"],
  ["Tim Taylor", "Television Host/Handyman"],
  ["Will Smith", "Student"],
  ["Dana Scully", "FBI Agent"]
]);

const tvCharacterObject = Object.groupBy(tvCharacters);

console.log(tvCharacterObject);
```
