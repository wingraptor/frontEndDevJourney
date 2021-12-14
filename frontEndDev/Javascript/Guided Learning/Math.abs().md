## Math.abs()

This method returns an absolute value of a number. It returns x if x is positive or 0, and the negation of x if x is negative (that is, positive x).

```js
function difference(a, b) {
  return Math.abs(a - b);
}

console.log(difference(3, 5));
// expected output: 2

console.log(difference(5, 3));
// expected output: 2

console.log(difference(1.23456, 7.89012));
// expected output: 6.6555599999999995
```