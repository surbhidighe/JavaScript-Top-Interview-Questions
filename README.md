# JavaScript-Interview-Questions-
Top JavaScript interview questions

******************************In progress


| S.No  | Questions |
| ------------- | ------------- |
| 1 | [What is JavaScript](#1-what-is-javascript)
| 2 | [What are the different data types in JavaScript](#2-what-are-the-different-data-types-in-javascript)  |
| 3 | [What are the different ways to create an Object in JavaScript](#3-what-are-the-different-ways-to-create-an-object-in-javascript)  |
| 4 | [Difference between == and === operators](#4-difference-between--and--operators)  |
| 5 | [Is javascript single-threaded or multi-threaded](#5-is-javascript-single-threaded-or-multi-threaded)  |
| 6 | [What are arrow functions and its features](#6-what-are-arrow-functions-and-its-features)  |
| 7 | [What do you mean by Synthetic events](#7-what-do-you-mean-by-synthetic-events)  |
| 8 | [What is array destructuring](#8-what-is-array-destructuring)  |
| 9 | [Can we combine two arrays using any es6 operators](#9-can-we-combine-two-arrays-using-any-es6-operators)  |
| 10 | [Why javascript is dynamically typed language](#10-why-javascript-is-dynamically-typed-language)  |
| 11 | [Difference between Undeclared and Undefined](#11-difference-between-undeclared-and-undefined)  |
| 12 | [Difference between Null and Undefined](#12-difference-between-null-and-undefined)  |
| 13 | [What is Temporal Dead Zone](#13-what-is-temporal-dead-zone)  |
| 14 | [What is IIFE](#14-what-is-iife)  |
| 15 | [What is Hoisting](#15-what-is-hoisting)  |
| 16 | [What are Cookies](#16-what-are-cookies)  |
| 17 | [What is memoization](#17-what-is-memoization)  |
| 18 | [Difference between var, let and const](#18-difference-between-var-let-and-const)  |
| 19 | [What is a callback function](#19-what-is-a-callback-function)  |
| 20 | [Is it possible to have both local and global variables with the same name](#20-is-it-possible-to-have-both-local-and-global-variables-with-the-same-name) |
| 21 | [Difference between Local Storage and Session Storage](#21-difference-between-local-storage-and-session-storage)  |

### 1. What is JavaScript
* JavaScript is a scripting language used to create dynamic and interactive websites. It is supported by all major web browsers.
* JavaScript is basically a client-side scripting language but it can also be used on the server-side with the help of technologies such as Node.js.

### 2. What are the different data types in JavaScript
| Primitive   |Non-primitive |
| ------------- | ------------- |
| Boolean, NULL, undefined, BigInt, String, Number, Symbol  | Object, Array | 

### 3. What are the different ways to create an Object in JavaScript

##### a) Object Literals: A comma-separated set of name and value pairs that is wrapped inside curly braces.

```javascript
var person = {
    name: 'Surbhi',
    age: 25,
    occupation: 'Software Engineer'
}
```
##### b) Object.create method: TCreates a new object, by using an existing object as the prototype of the newly created object.

```javascript
const person = {
    name: 'Surbhi',
    age: 25,
    occupation: 'Software Engineer'
}

var info = Object.create(person);
console.log(info.name); // output - Surbhi
```
Here "person" is an existing object which is passed as a prototype to the newly created object "info"

##### c) Object constructor: Constructor function allows to create objects with the help of new keyword

```javascript
const person = new Person();
```

##### d) using ES6: We can create object using ES6 class feature

```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
}
  
let person = new Person('Surbhi');
  
console.log(person.name);  //output - Surbhi
```

### 4. Difference between “==” and “===” operators
* == : While comparing two operands, checks for only value
* === : While comparing two operands, checks for value as well as data type

### 5. Is javascript single-threaded or multi-threaded
* JavaScript is Single-threaded

### 6. What are arrow functions and its features
Arrow functions were introduced in ES6 (ECMAScript 2015) and provide a simpler and compact way to write functions. They are also called “fat arrow functions”
###### Syntax
```javascript
const functionName = (something) => {
  return something;
}
```
###### Features of arrow functions
1. They use a concise syntax which makes them shorter and easier to read as compared to traditional function expressions
2. They do not bind their own this value, but instead inherit the this value from the enclosing lexical scope (i.e., the scope in which it is defined)
3. They do not have "prototype" property and hence cannot be used as a constructor
4. If the arrow function body consists of a single expression, that expression will be implicitly returned, without the need for a return statement.
5. If an arrow function has only one parameter, the parentheses around the parameter list can be omitted.

### 7. What do you mean by Synthetic events
Synthetic events are objects that act as a cross-browser wrapper around a browser's native event. It has the same interface as the browser's native event, including stopPropagation() and preventDefault(), except the events work identically across all browsers.

### 8. What is array destructuring
Array destructuring is a unique feature in JavaScript that allows you to extract array's value into new variables. For e.g.,
```javascript
const arr = [1,2,3];
const [num1, num2, num3] = arr;
console.log(num1); // output =====> 1
console.log(num2); // output =====> 2
console.log(num3); // output =====> 3
```

### 9. Can we combine two arrays using any es6 operators
* Yes, using Spread Operators
```javascript
const arr1 = [1,2,3,4];
const arr2 = [5,6];
const arr3 = [...arr1, ...arr2]
console.log(arr3) // output =====> [1,2,3,4,5,6]
```

### 10. Why javascript is dynamically typed language
JavaScript is a dynamically typed language, because the type of a variable is determined at runtime based on the value it holds. For e.g.,
```javascript
var variable_one = "surbhi"  // "string" datatype is determined at runtime
var variable_two = 20        // "number" datatype is determined at runtime
```

### 11. Difference between Undeclared and Undefined
**Undeclared -** A variable that has not been declared or doesn't exists in the code
```javascript
console.log(a); // output =====> ReferenceError: a is not defined
```
**Undefined -** A variable that has been declared but not assigned a value yet
```javascript
let a;
console.log(a); // output =====> undefined
```

### 12. Difference between Null and Undefined
**Null -** Null means an empty value or a blank value. It is used to represent an intentional absence of value. 
```javascript
let demo = null;
console.log(demo); // output =====> null
```

**Undefined -** Undefined means the variable has been declared, but its value has not been assigned yet.
```javascript
let demo;
console.log(demo); // output =====> undefined
```

### 13. What is Temporal Dead Zone
A "let" or "const" variable is said to be in a "temporal dead zone" (TDZ) from the start of the block until code execution reaches the line where the variable is declared and initialized.

In JavaScript, variables declared with let or const are not hoisted to the top of the block scope. If you try to access a variable before it is declared, a ReferenceError will be thrown.
```javascript
{
  // TDZ for name variable starts here
  console.log(name); // ReferenceError
  let name = "surbhi"; // End of TDZ for name
}
```

### 14. What is IIFE
IIFE stands for Immediately Invoked Function Expression. It is a JavaScript function that is executed as soon as it is defined. 

An IIFE is typically written as an anonymous function expression that is enclosed within a set of parentheses, followed by another set of parentheses that call the function. For e.g.,
```javascript
(function() {
  // code goes here
})();
```

### 15. What is Hoisting
Hoisting is a default behavior in JavaScript where variable and function declarations are moved to the top of the current scope

**Variable hoisting**
```javascript
console.log(a);  // output =====> undefined
var a = 10;
```
The output of above code will be undefined because the declaration of "a" is hoisted to the top of the scope, but the initialization happens later in the code.

```javascript
a=10;
console.log(a);  // output =====> 10
var a;
```
The output of above code will be 10 because the variable "a" is hoisted to the top of the scope and its value is assigned before console.log

**Function hoisting**
```javascript
demo();  // demo console
function demo() {
	console.log('demo console');  //
}
```
The output of above code will be "demo console" because the function declaration is hoisted to the top of the scope, allowing it to be called before it is declared in the code.
```diff
**Note**
+ Only function declarations are hoisted, not the function expressions.
+ Only the declaration is hoisted, not the initialization. 
```

### 16. What are Cookies
In javascript, a cookie is a piece of data, stored in small text files, on the user's computer by the browser.
Cookies are set, read and deleted using the document.cookie property

```javascript
//**Set a cookie**
document.cookie = "username=surbhi";

//**Read a cookie**
let cookie_variable = document.cookie; 

//**Delete a cookie** (set the expiration date to a past date/time)
document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
```

### 17. What is memoization
Memoization is a technique used in JavaScript to optimize the performance of functions by caching the results of expensive function calls, based on their input parameters.
For e.g., If a function is called multiple times with the same input parameters, then it will perform the same calculations each time. By memoizing the function, we can use the cached result.

```js
function memoizedAdd(num1, num2) {
  let cache = {};
  return function (a, b) {
    const key = num1 + ' and ' + num2;
    if (key in cache) {
      console.log('Retrieving from cache:', key);
      return cache[key];
    } else {
      console.log('Calculating result:', key);
      const result = num1 + num2;
      cache[key] = result;
      return result;
    }
  };
}

const add = memoizedAdd();
console.log(add(2, 3)); // "Calculating result:", "2 and 3", output=====> 5
console.log(add(2, 3)); // "Retrieving from cache:", "2 and 3" output=====> 5
```

### 18. Difference between var, let and const
In javascript, there are 3 ways to declare a variable - var, let, and const. However, they have some differences in their behavior and scope.
| var | let | const |
| --- | --- | --- |
| Function scoped | Block scoped | Block scoped | 
| Can be re-declared in the same scope | Can not be re-declared in the same scope | Can not be re-declared in the same scope |
| Can be updated in the same scope | Can be updated in the same scope | Can not be updated in the same scope |
| Hoisted to the top of their scope | Hoisted to the top but are not initialized | Hoisted to the top but are not initialized |
| Can be declared without being initialized |Can be declared without being initialized | Can not be declared without being initialized |

### 19. What is a callback function
A callback function is a function that is passed as an argument to another function. The function that receives the callback as an argument can then invoke the callback at any time during its execution. 
```js
function message(callback) {
    console.log('Hi, i am message function');
    callback();
}
// callback function
function callBackFun() {
    console.log('Hey, I am a callback function');
}
// passing callback function as an argument to message function
message(callBackFun);
```

### 20. Is it possible to have both local and global variables with the same name
Yes, we can have both with the same name. But when we do this, the local variable will take precedence over the global variable within the scope of the function or block of code in which it is declared.

However, outside of that scope, the global variable will still be accessible using its name.

```js
let a = 10;
function Demo(){
let a = 20;
console.log(a, "local scope");
}
Demo();
console.log(a, "global scope");
```

### 21. Difference between Local Storage and Session Storage
Local storage and session storage are web storage provided by web browsers to store data on the client-side

**Local Storage** - Data stored in local storage will persist even after the browser window is closed or the user navigates away from the website and it is available across all windows and tabs of the same origin.

**Session Storage** - Data stored in session storage will be deleted when the browser window is closed or the session ends and it is available only within the same window or tab that created the data.

******************************In progress


