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


******************************In progress


