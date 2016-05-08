---
layout: post
title: ES2015 Arrow Functions
---


## What are arrow functions?

An arrow function, in javascript, is a function declaration using the arrow syntax (=>).  

```javascript
// Function declared with arrow syntax
const arrowFunction = () => console.log(2);

//logs 2
arrowFunction()

//logs 2 every second
setInterval(() => {
    return 2;
  }, 1000);

//When you have only one expression in the function,
//you don't need curly braces or a return statement

//logs 2 every second
setInterval(() => console.log(2), 1000);

```
## What makes arrow functions different than named functions?

### 1) Arrow functions are easier to read (particularly when the function is short).

Compare

```javascript

setInterval(() => console.log(2), 1000);

```
to

```javascript

setInterval(function() {
  console.log(2)
  }, 1000);

```

### 1) Arrow functions change how the keyword *this* works.

If you're not familiar with how *this* works then I suggest that you read up on it and come back. Here are some great explanations.  
[Kyle Simpson](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/ch1.md)
[Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
[Mike West](http://www.digital-web.com/articles/scope_in_javascript/)
[Sitepoint](http://www.sitepoint.com/inner-workings-javascripts-this-keyword/)



```javascript
//In the global context, this refers to the global object
this



```
