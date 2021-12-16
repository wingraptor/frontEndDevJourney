---
creation date: 2021-12-13 16:29
modification date: Tuesday 14th December 2021 19:12:37
tags: methods, javascript, array
---


# String.substring()

**_Checklist_**

- [x] Add Notes
- [x] Add to Anki
- [x] Update tags (Example: arrays, math)
- [x] Remove TODO tag

This function returns the part of the `string` that lies between the `startIndex` and the `endIndex`, or to the end of the `string`.


---

## Syntax

```js

someString.substring(indexStart, indexEnd);


```

### Parameters
- `indexStart`: the index of the first character to be included in the returned string.
- `indexEnd`(optional): the index of the first character NOT to be included in the returned string. 
- 

### Return Value

string composed of a substring of the original string. 



---

## Description

substring() extracts the characters from `indexStart` up to but NOT including the `indexEnd`.  In particular:

-   If `indexEnd` is omitted, `substring()` extracts characters to the end of the string.
-   If `indexStart` is equal to `indexEnd`, `substring()` returns an empty string.
-   If `indexStart` is greater than `indexEnd`, then the effect of `substring()` is as if the two arguments were swapped; See example below.

Any argument value that is less than `0` or greater than `stringName.length` is treated as if it were `0` and `stringName.length`, respectively.

Any argument value that is [`NaN`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN) is treated as if it were `0`.

## Examples
```js
let anyString = 'Mozilla'

// Displays 'M'
console.log(anyString.substring(0, 1))
console.log(anyString.substring(1, 0))

// Displays 'Mozill'
console.log(anyString.substring(0, 6))

// Displays 'lla'
console.log(anyString.substring(4))
console.log(anyString.substring(4, 7))
console.log(anyString.substring(7, 4))

// Displays 'Mozilla'
console.log(anyString.substring(0, 7))
console.log(anyString.substring(0, 10))
```


NB: substring can be used to extract the final characters of a string by using someString.length - x. Where x is the number of characters from the end of the string that you want included in the returned substring. 


```js
// Displays 'illa' the last 4 characters
let anyString = 'Mozilla'
let anyString4 = anyString.substring(anyString.length - 4)
console.log(anyString4)

// Displays 'zilla' the last 5 characters
let anyString = 'Mozilla'
let anyString5 = anyString.substring(anyString.length - 5)
console.log(anyString5)
```



---


## Resources
- [String.prototype.substring() - JavaScript | MDN (mozilla.org)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/substring)

