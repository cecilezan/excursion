---
Title: '.groupBy()'
Description: 'Groups items by a string value.'
Subjects:
  - 'Web Development'
Tags:
  - 'Methods'
  - 'Objects'
CatalogContent:
  - 'introduction-to-javascript'
  - 'paths/full-stack-engineer-career-path'
---

The **`.groupBy()`** method groups items according to the values (a string) returned by a callback function (link codecademy.com/ressources/docs/javascript/callbacks). The returned value of the **`.groupBy()`** method is a null-prototype object : it doesn't inherit any object methods. (link vers https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/groupBy)

## Syntax

```pseudo
Object.groupBy(items, callfunc);
```

The `items` is usually an Array .
The `callfunc` is a callback function with 2 or 3 arguments and have to return a string.

## Example

Grouping users by their year of subscription.

```js
const subs = [
{ userName: 'Lisa', yearSub: 2022 },
{ userName: 'Akim', yearSub: 2020 },
{ userName: 'Lola', yearSub: 2020 },
];

const subsByYear = Objets.groupBy(subs, user => {
  return user.yearSubs;
});
/* =>  { 2020: [{ userName: 'Akim', yearSubs: 2020 },
{ userName: 'Lola', yearSubs: 2020 },
 
], even: [2, 4] }

console.log(newObject);*/
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
