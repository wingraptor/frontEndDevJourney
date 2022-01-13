# AKA Conditional Operator

Only operator that takes three operands and is often used as a shortcut for if statements.

**Syntax** ^9672fa

```js
condition ? expr1 : expr2
```
If  `condition`  is  `true`, the operator evaluates to  `expr1`; otherwise, it evaluates to `expr2`.

**Example**

```js
var age = 26;
var canDrinkAlcohol = (age > 21) ? "True, over 21" : "False, under 21";
console.log(canDrinkAlcohol); // "True, over 21"
```

In above example, 'No' is logged to console because the variable isMarried is given the Boolean value of false and therefore the else statement is logged.

*NB: You cannot include a return statement inside a conditional operator*

Note that the ternary operator is used on expressions and not statements. This means that you cannot put `return` inside there - if you need to use in `if` statement. That being said, you can move the return outside to return the value given by the expression.

```js
return conditional ? false : true
``` 

You cannot use a conditional operator to return in one case but not the other, because `return` is a _statement_, and the conditional operator's operands are _expressions_, not statements. In JavaScript, you can use an expression where a statement is expected (it becomes an _ExpressionStatement_), but not vice-versa. *Expressions* in javascript must evaluate to a something (E.g. `1 + 1`) while *statements* perform an action. `expr1` and `expr2` in [[ternaryOperator#^9672fa | syntax example]]  above most evaluate to something so that the ternary operator itself can evaluate to a value. This value is either the value of expr1 or expr2. 

## References
https://stackoverflow.com/a/35231691
https://stackoverflow.com/a/30343606

conditional ? expr1 : expr 2;