Link: https://www.udemy.com/share/101XjU3@Vp5NgCTTVKKdf03z6ZJVAtVo3l9E9iBBLnsWwDwUVhIK3Jtqc-haWPO7PTIRR5Ep_Q==/

## Syntax Parser:
>Program that reads your code and determines what it does and if the grammar is valid.

## Lexical Environment
>Where something sits physically in the code you write; where it is and what surrounds it

Lexical means 'having to do with the words or grammar.'

```js

function hello() {

var a = 'hello world'  // var a is 'in' hello function lexical environment

}

```
## Execution Context
>A wrapper to help manage the code that is running.  

There are lots of lexical environments. Which one is currently running is managed via execution contexts. It can contain things beyond what you've written in your code. 

## Name/Value Pair
>A Name which maps to a unique value. 

The name may be defined more than once, but only can have one value in any given **context**. Additionally, that value may be more name/value pairs. 

```js

let x = 21

// x = name and value = 21
```

## Object
>Collection of name/value pairs (In Javascript)


## Global Environment and the Global Object
> _'Global'_ refers to code that is **not in a function**, its lexically not found in a function and is accessible to everything in my code.

When running JS code in a browser, the JS engine creates the **Global Execution Context** which contains the **Global Object** and the **this** variable.  The **Global Object** and **this** both have as their value the **Window Object**. 

![[Pasted image 20220425122618.png]]



## Hoisting 
> Process by which space is set up in memory for variables and  functions.

This process occurs during the **Creation Phase** of setting up the Execution Context.  This process occurs before the line-by-line execution of code in the execution phase. 

![[Pasted image 20220425141848.png]]

Note that during the **Creation Phase** functions are stored fully in memory while variables are assigned the value `undefined`. Variables are only assigned a value during the execution phase. 
