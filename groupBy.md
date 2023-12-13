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

The **`.groupBy()`** method groups items of a given iterable according to the string values returned by a provided callback function. This callback function will determine the group name .The returned value of **`.groupBy()`** method is a null-prototype object, it doesn't inherit any object methods from **`object.prototype`**.

## Syntax

```pseudo
Object.groupBy(iterable, callfunc);
```

The `iterable` is usually an Array .
The `callfunc` is callback function with 2 returns a string, .

## Example

Creating an object from an array.

```js
const subs = [
{ userName: 'czzanco', yearSubs: 2022 },
{ userName: 'czzanco2', yearSubs: 2020 },
{ userName: 'czzanco3', yearSubs: 2020 },
];

const subsByYear = subs.groupBy(user => {
  return user.yearSubs;
});
// =>  { 2020: [{ userName: 'czzanco2', yearSubs: 2020 },
{ userName: 'czzanco3', yearSubs: 2020 },
 
], even: [2, 4] }

console.log(newObject);
```

The output would be:

```shell
{ '0': 'Los Angeles', '1': 'Toronto', '2': 'Paris' }
```

## Codebyte Example

Following is a runnable example that demonstrates the `.groupBy()` method.

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
