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
| 22 | [Difference between forEach() and map()](#22-difference-between-foreach-and-map)  |
| 23 | [What is rest operator](#23-what-is-rest-operator)  |
| 24 | [What is spread operator](#24-what-is-spread-operator)  |
| 25 | [Difference between async and defer](#25-difference-between-async-and-defer)  |
| 26 | [What is Nullish coalescing operator](#26-what-is-nullish-coalescing-operator)  |
| 27 | [What is the difference between a parameter and an argument](#27-what-is-the-difference-between-a-parameter-and-an-argument)  |
| 28 | [What is a closure](#28-what-is-a-closure)  |
| 29 | [Difference between function declaration and function expression](#29-difference-between-function-declaration-and-function-expression)  |
| 30 | [What are the different ways to create an array in javascript](#30-what-are-the-different-ways-to-create-an-array-in-javascript)  |
| 31 | [Difference between window and document in javascript](#31-difference-between-window-and-document-in-javascript)  |
| 32 | [What is strict mode in javaScript](#32-what-is-strict-mode-in-javascript)  |
| 33 | [What are the different ways to empty an array in javascript](#33-what-are-the-different-ways-to-empty-an-array-in-javascript)  |
| 34 | [What is NaN in javascript](#34-what-is-nan-in-javascript)  |
| 35 | [Javascript naming convention](#35-javascript-naming-convention)  |
| 36 | [Difference between call(), apply() and bind()](#36-difference-between-call-apply-and-bind)  |
| 37 | [What is the use of isNaN function](#37-what-is-the-use-of-isnan-function)  |
| 38 | [What is 'this' keyword in javascript](#38-what-is-this-keyword-in-javascript)  |
| 39 | [How do we add comments in javascript](#39-how-do-we-add-comments-in-javascript)  |
| 40 | [What is the use of typeof operator](#40-what-is-the-use-of-typeof-operator)  |
| 41 | [Is JavaScript case-sensitive](#41-is-javascript-case-sensitive)  |
| 42 | [Difference between push() and unshift()](#42-difference-between-push-and-unshift)  |
| 43 | [Difference between pop() and shift()](#43-difference-between-pop-and-shift)  |
| 44 | [Different ways to access DOM elements in js](#44-different-ways-to-access-dom-elements-in-js)  |
| 45 | [What are promises](#45-what-are-promises)  |
| 46 | [What is a prototype](#46-what-is-a-prototype)  |
| 47 | [What is a callback hell](#47-what-is-a-callback-hell)  |
| 48 | [What is an event loop](#48-what-is-an-event-loop)  |
| 49 | [ES6 and its features](#49-es6-and-its-features)  |
| 50 | [Difference between function and method](#50-difference-between-function-and-method)  |
| 51 | [What is aync and await](#51-what-is-aync-and-await)  |


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
```js
console.log(1=="1");  // output=>>>>>>>>> true
```
* === : While comparing two operands, checks for value as well as data type
```js
console.log(1==="1");  // output=>>>>>>>>> false
```

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
	console.log('demo console'); 
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
console.log(add(2, 3)); // "Calculating result:", "2 and 3", output ========> 5
console.log(add(2, 3)); // "Retrieving from cache:", "2 and 3" output ========> 5
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

### 22. Difference between forEach() and map()
map() and forEach() are array methods that can be used to iterate over an array.
**map()** 
1. map() method receives a function as an argument, executes it once for each array element and returns a new array
2. It is generally used when we need to modify/change data, because it returns a new array with the transformed data
3. It is chainable because we can attach sort(), filter() etc. after performing a map() method on an array

```js
const arr = [1,2,3,4,5]
let result = arr.map(x => x * x)
console.log(result)   // output ========> [1,4,9,16,25]
```

**forEach()** 
1. forEach() method receives a function as an argument, executes it once for each array element but returns undefined.
2. It is generally used when we just need to iterate over an array 
3. It is not chainable

```js
const arr = [1,2,3,4,5]
let result = arr.forEach(x => x * x)
console.log(result)   // output ========> undefined
```

### 23. What is rest operator
1. The rest operator was introduced in ES6 (ECMAScript 2015) and it is represented by three dots (...)
2. It is used in function parameters and allows you to represent an indefinite number of arguments as an array

```js
function addition(...numbers) {
  return numbers.reduce((a,b)=>a+b);
}
console.log(addition(1, 2, 3, 4)); // output ========> 10
```

3. It collects all the remaining arguments passed to a function into an array

```js
function profile(name, designation,...location) {
  return location
}
console.log(profile("surbhi","SE","India","Indore","M.P")); // output ========> ["India", "Indore", "M.P"]
```

### 24. What is spread operator
1. The spread operator was introduced in ES6 (ECMAScript 2015) and it is represented by three dots (...)
2. It allows an iterable to be spread into individual elements
```js
const arr = [1, 2, 3, 4,5];
console.log(...arr); // output ======> 1, 2, 3, 4, 5
```
3. It can be used to copy the elements of an existing array into a new array, or to concatenate arrays
```js
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const arr3 = [...arr1, ...arr2];
console.log(arr3);  // output =======> [1, 2, 3, 4, 5, 6]
```
4. It can be used to copy the properties of an existing object into a new object
```js
const obj1 = { a:1, b:2 };
const obj2 = { c:3 };
const obj3 = { ...obj1, ...obj2 }; 
console.log(obj3); // output ========> { a: 1, b: 2, c: 3 }
```

### 25. Difference between async and defer
async and defer are the attributes used with the script tag in HTML to load javaScript files.

**Async** - The script is loaded in parallel to the HTML parsing, and executed as soon as it is available i.e., it executes the script immediately after it is loaded. It can be useful for scripts that don't depend on the DOM. 

**Defer** - The script is loaded in parallel to the HTML parsing, and executed after the page is completely loaded i.e., it waits until the page has finished parsing. It can be useful for scripts that depend on the DOM. 

### 26. What is Nullish coalescing operator
1. The nullish coalescing (??) operator is a logical operator
2. It allows you to check if a value is either null or undefined
3. It returns its right-hand side operand if its left-hand side operand is null or undefined, otherwise returns its left-hand side operand
```js
console.log((null || undefined) ?? "foo"); // output ========>  "foo"
console.log("hello" ?? "foo");		   // output ========>  "hello" 
```

### 27. What is the difference between a parameter and an argument
**Parameter** - A parameter is a variable that is defined during a function declaration or definition. It represents a value that the function or method expects to receive as an input.

**Argument** - An argument is the actual value that is passed to a function or method when it is called. 
```js
function Demo(parameter1, parameter2){
 something------
 something------
}
Demo(argument1, argument2);
```

### 28. What is a closure
A closure is a combination of a function and the environment in which it was created(lexical scope). It gives you access to an outer function's scope from an inner function even if the outer function has returned
```js
function Demo() {
  let name = "Surbhi";
  function displayName() {
    console.log(name);
  }
  return displayName;
}

const result = Demo();
result();
```

### 29. Difference between function declaration and function expression
**Function Declaration**
1. A function declaration defines a function using the function keyword, followed by the function name
2. We can call a function, declared using a function declaration, before it is defined. Because it is hoisted to the top of its scope
3. It does not require a variable assignment 
```js
function Message() {
  console.log("Welcome Message"); // output ========> Welcome Message
}
Message();
```

**Function Expression**
1. A function Expression is similar to a function declaration without the function name
2. We can not call a function, declared using a function expression, before it is defined
3. It can be stored in a variable assignment
```js
const Message = function() {
  console.log("Welcome Message"); // output ========> Welcome Message
}
Message();
```

### 30. What are the different ways to create an array in javascript
1. **Using the array literal notation**
```js
const arr = [1,2,3,4,5];
```
2. **Using the Array() constructor**
```js
const arr = new Array(1, 2, 3, 4, 5);
```

### 31. Difference between window and document in javascript
**window object** - window is the topmost object. It represents the browser window or tab containing a DOM document. It provides various properties and methods to manipulate the browser window, such as window.alert(), window.confirm(), and window.location. 

**document object** - document represents the HTML document that is being displayed in the window. It provides properties and methods to manipulate the HTML elements in the document, such as document.title, document.getElementById(), and document.createElement().

### 32. What is strict mode in JavaScript
1. Strict mode was introduced in ECMAScript 5
2. It performs additional checks on your code to prevent certain types of bugs and errors that may go unnoticed e.g., using undeclared variables, using duplicate property names in objects
3. It can be enabled at either the global level or at the function level
4. It can't be apply to block statements enclosed in {} braces
5. To invoke strict mode, put the exact statement “use strict”; or ‘use strict’; 

### 33. What are the different ways to empty an array in javaScript
**Using length property**
```js
let arr = [1, 2, 3, 4, 5];
arr.length = 0;
console.log(arr); // output ========> []
```

**Assigning it to a new empty array**
```js
let arr = [1,2,3,4,5];
arr = [];
console.log(arr); // output ========> []
```

**Using the splice() method**
```js
let arr = [1, 2, 3, 4, 5];
arr.splice(0, arr.length);
console.log(arr); // output ========> []
```

### 34. What is NaN in javascript
1. In Javascript, NaN stands for "Not a Number"
2. It is a global property that represents an unrepresentable mathematical result
3. It is returned when a mathematical operation has no meaningful result. E.g., dividing zero by zero, multiplying/dividing a non-numeric value by a number etc.

```js
console.log(0/0);                  // output ========> NaN
console.log("a"*1);                // output ========> NaN
console.log("a"/1)		   // output ========> NaN
console.log(Math.sqrt(-1));	   // output ========> NaN
console.log(parseInt("blabla"));   // output ========> NaN
```

### 35. Javascript naming convention
1. Use camelCase (lowercase for the first word, then uppercase for subsequent words) for variable and function names
2. Use PascalCase for class names (uppercase for the first letter of each word)
3. Use "is" or "has" as prefixes for boolean variables
4. Use UPPERCASE for constants 
5. Use descriptive and meaningful names for your variables, functions, and classes.

```js
//variable
let firstName = "Surbhi";

//function
function displayName() {
 return "Surbhi Dighe";
}
displayName();

//boolean
let isLoading = false;
let hasName = true;

//constants
let SECONDS = 60;

//class
class DisplayName { 
  constructor(firstName, lastName) { 
    this.firstName = firstName; 
    this.lastName = lastName; 
  }
}
var name = new DisplayName('Surbhi', 'Dighe');
```

### 36. Difference between call(), apply() and bind()
call(), apply(), and bind() methods are used to attach a function into an object and call the function as if it belonged to that object. 

**call()**  - call() is used to invoke a function immediately with a specified *this* value and allows you to pass the arguments one by one
```js
let person = {name: 'Surbhi'};
function printName(message) {
    console.log(message + ' ' + this.name);   // output ========> "Hello Surbhi"
}
printName.call(person, 'Hello'); 
```
**apply()** - apply() is used to invoke a function immediately with a specified *this* value and allows you to pass the arguments as an array
```js
let person = {name: 'Surbhi'};
function printName(message) {
    console.log(message + ' ' + this.name);   // output ========> "Hello Surbhi"
}
printName.apply(person, ['Hello']); 
```
**bind()** - bind() returns a new function (which can be invoked anytime), with a specified *this* value and allows you to pass in arguments
```js
let person = {name: 'Surbhi'};
function printName(message) {
    console.log(message + ' ' + this.name);   // output ========> "Hello Surbhi"
}
let sayHello = printName.bind(person, "Hello"); 
sayHello();
```

### 37. What is the use of isNaN function
isNaN() is a built-in JavaScript function. It takes a single argument and returns true if the argument is not a number, otherwise it returns false.
```js
let num1 = 5;
let num2 = "hi";

console.log(isNaN(num1));	// output ========> false
console.log(isNaN(num2));	// output ========> true
```

### 38. What is 'this' keyword in javascript
The value of 'this' is determined by the context in which it is used. In general, 'this' keyword refers to the object it belongs to.
The 'this' keyword in JavaScript can have different values depending on where it is used -
1. If it is used inside a method, then it refers to the object that it belongs to
2. If it is used inside any function or alone (i.e outside any function or method), then it referes to the global object
3. If it is used in the context of an event handler, such as a click event, then it refers to the element that triggered the event

### 39. How do we add comments in javascript
**Single-line comments** - Add comments using 2 forward slashes // 
```js
// this is a single line comment
```
**Multi-line comments** - Enclose the text between /* and */
```js
/*
This is a
multiline comment
example
*/
```

### 40. What is the use of typeof operator
The typeof operator returns a string that indicates the data type of the variable/value.
```js
let var1 = "Surbhi";
let var2 = 10;
console.log(typeof var1);	// output ========> "string"
console.log(typeof var2);       // output ========> "number"
console.log(typeof "hello");	// output ========> "string"
console.log(typeof 2);		// output ========> "number"
console.log(typeof true);	// output ========> "boolean"
```

### 41. Is JavaScript case-sensitive
Yes, JavaScript is a case-sensitive language. For e.g., the variables firstName and firstname are considered to be two different variables.
```js
let firstName = "Surbhi";
console.log(firstname);         // output ========> Uncaught ReferenceError: firstname is not defined
```

### 42. Difference between push() and unshift()
Both are used to add elements to an array, but they add elements in different ways.

**push()** - It adds one or more elements to the end of an array and returns the new length of the array.
```js
let arr = [1,2,3,4];
let newArr = arr.push(5,6,7);
console.log(newArr); 		// output ========> 7
console.log(arr);		// output ========> [1, 2, 3, 4, 5, 6, 7]
```
**unshift()** - It adds one or more elements to the beginning of an array and returns the new length of the array.
```js
let arr = [1,2,3,4];
let newArr = arr.unshift(5,6,7);
console.log(newArr);		// output ========> 7
console.log(arr);		// output ========> [5, 6, 7, 1, 2, 3, 4]
```

### 43. Difference between pop() and shift()
Both are used to remove elements from an array, but they remove elements in different ways.

**pop()** - It removes the last element of an array and returns the removed element.
```js
let arr = [1,2,3,4];
let newArr = arr.pop();
console.log(newArr);		// output ========> 4
console.log(arr);		// output ========> [1,2,3]
```

**shift()** - It removes the first element of an array and returns the removed element.
```js
let arr = [1,2,3,4];
let newArr = arr.shift();
console.log(newArr);		// output ========> 1
console.log(arr);		// output ========> [2,3,4]
```

### 44. Different ways to access DOM elements in js
*getElementById* - This method is used to get an element by its ID.

*getElementsByClassName* - This method is used to get a collection of elements by their class name.

*getElementsByTagName* - This method is used to get a collection of elements by their tag name.

*querySelector* - This method is used to get the first element that matches a specified CSS selector.

*querySelectorAll* - This method is used to get a collection of elements that match a specified CSS selector.

### 45. What are promises
In JavaScript, promises are used to handle asynchronous operations. The code does not directly or immediately return a value. Instead, it returns a promise that, it will eventually get resolved or rejected. 
A promise can have three possible states:

*Pending* - The initial state, before the promise is resolved or rejected.

*Resolved* - When a promise has been successfully completed and a value is returned.

*Rejected* - When a promise has been failed and an error is returned.

```js
let promise = new Promise((resolve, reject) => {
  const result = AsynchronousTaskFunction();
  if (result) {
    resolve(result);
  } else {
    reject(new Error('Operation failed'));
  }
});

promise.then(result => {
  console.log(result, "It is resolved");
}).catch(error => {
  console.error(error, "It is rejected");
});
```

### 46. What is a prototype
Every object in JavaScript has a built-in property, which is called its prototype. All JavaScript objects inherit properties and methods from a prototype.

It allows us to add properties and methods to all instances of a given object type.
```js

function Person(name, age) {
  this.name = name;
  this.age = age;
}
Person.prototype.city = "Indore"
var person1 = new Person('John', 30);
console.log(person1);			
```

### 47. What is a callback hell
Callback hell is a situation in which callback functions are nested inside each other at several levels, making the code difficult to read, write, and maintain.
```js
asyncFunc1(function(response1) {
  asyncFunc2(response1, function(response2) {
    asyncFunc3(response2, function(response3) {
      asyncFunc4(response3, function(response4) {
       asyncFunc5(response4, function(response5) {
        // ... and so on
        });
      });
    });
  });
});
```

### 48. What is an event loop
The event loop is a key mechanism in JavaScript that provides an illusion of being multithreaded despite being single-threaded, allowing for non-blocking, asynchronous processing of events and callbacks.It monitors both the callback queue and the call stack. 

If the call stack is not empty, the event loop waits until it is empty 

If the call stack is empty it places the next function from the callback queue to the call stack


### 49. ES6 and its features
ES6 stands for ECMAScript 6, also known as ECMAScript 2015. It is the sixth major version of the ECMAScript language specification for JavaScript. Below are some of the significant features of ES6

*Arrow functions, template literals, block-scoped variables (let and const), default function parameters, array and object destructing, promises, rest and spread operators, classes.*

### 50. Difference between function and method
**method** - A method is a function associated with an object. 
```js
let obj = {
name:"Surbhi",
greet: function(){     
return `Hi ${this.name}`
}
}
console.log(obj.greet());
```
**function** - A function is a self-contained block of code that can be defined and called independently of any object.
```js
function sum(a, b) {
  return a + b;
}
sum(2,4);
```

### 51. What is aync and await
async/await is a feature in JavaScript that allows us to write asynchronous code that looks more like synchronous code. "await" works only inside "async" functions

"async" ensures that a function returns a promise and "await" pause the execution of the function until a promise is resolved or rejected. 
```js
const getData = async () => {
  const response = await fetch('https://api.openweathermap.org/data/2.5/weather?q=New%20York&appid=YOUR_API_KEY');
  const data = await response.json();
  console.log(data);
}
getData();
```


