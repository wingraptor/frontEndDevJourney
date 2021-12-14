Only operator that takes three operands and is often used as a shortcut for if statements.

**Syntax**

```js
condition ? expr1 : expr2
```
If  `condition`  is  `true`, the operator returns the value of  `expr1`; otherwise, it returns the value of  `expr2`.

**Example**

```js
var age = 26;
var canDrinkAlcohol = (age > 21) ? "True, over 21" : "False, under 21";
console.log(canDrinkAlcohol); // "True, over 21"
```

In above example, 'No' is logged to console because the variable isMarried is given the Boolean value of false and therefore the else statement is logged.