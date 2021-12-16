# Array.forEach() Method

## Description

This is a built-in Array Function ([[Array Methods | Array Method ]]) for iterating over an [[Array]].

---


## Syntax

.forEach takes a callback function, that callback function is expected to have at least 1, but up to 3, arguments. 

```js
arr.forEach(function(el, i, arr), thisValue)
```

---

### Parameters

The parameters are in a specific order:

-   The first one (`el` in example) represents each element in the array (per loop iteration) that .forEach was called on. This is a placeholder name and can be anything that you want it to be.
    
-   The second (`i` in example) represents the index of said element. (**Optional**)
    
-   The third (`arr` in example) represents the array that .forEach was called on (it will be the same for every iteration of the loop). **Optional.**
-  
-   The fourth (`thisValue`) represents the value passed to the function as its `this` value. 
    
	
	### Return Value
	
	`undefined`
	
	
---

## Examples

You have a couple options when calling .forEach on an array:

You can pass in an anonymous function:

### Example 1

```js
[1,2,3].forEach(function(el, i, arr) {
  console.log(el, i, arr);
}); // I interpret this as meaning; for each element in the array carry out the function on that element.

```

Or you can pass in a pre-written, named function.

### Example 2

```js
function logNums(el, i, arr) {
  console.log(el, i, arr);
}

[1,2,3].forEach(logNums); OR arr.forEach(logNums); 
// Calling the forEach function using the lognums anonymous function
// as a argument. arr is just a generic array name
```

Notice how in the second example we don't invoke logNums when passing it into .forEach. We simply pass in the function name. We don't need to invoke the logNums function, .forEach does that for us. In fact, it invokes the function multiple times, once for every element inside of the array.

---

## Further Examples

```js
var colors = ["red", "orange", "yellow", "green"];

colors.forEach(function(color){
   //color is a placeholder, call it whatever you want. 
     console.log(color);   
});

```


In the example above each item from the array and logs it to the console.

```js
var colors = ["red", "orange", "yellow", "green"];

colors.forEach(function(){
   //color is a placeholder, call it whatever you want. 
     console.log("stuff");   
});

```

In the example above "stuff" is logged to the console 4 times,  **once for each item in the array. For each item in the array an item is logged.**

```js
const numbers = [65, 44, 12, 4];  
numbers.forEach(myFunction)  
  
function myFunction(item, index, arr) {  
 arr[index] = item * 10;  
}

```
---


### forEach With String

Have to convert string to array by using the [[Spread Operator]].



## Resources
- [JavaScript Array forEach() Method (w3schools.com)](https://www.w3schools.com/jsref/jsref_foreach.asp)
