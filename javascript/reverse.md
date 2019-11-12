# Reverse an array

A super elegant variant to reverse an array in JavaScript:

```javascript
const reverse = ([value, ...rest]) =>
  value !== undefined ? [...reverse(rest), value] : [];
```

Example / Usage:

```javascript
let listOfNumbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0];
let reversedNumbers = reverse(listOfNumbers);

console.log(reversedNumbers); // [0, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```
