---
layout: post
title: ES2015 Arrow Functions
---


### What are arrow functions?

An arrow function, in javascript, is a function declaration using the arrow syntax (=>).  

#### Examples of arrow functions
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
### What makes arrow functions different than named functions?

Arrow functions are easier to read (particularly when the function is short).

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
