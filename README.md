# JavaScript-Interview-Questions-
Top JavaScript interview questions

******************************In progress


| S.No  | Questions |
| ------------- | ------------- |
| 1  | [What is JavaScript](#1-what-is-javascript)
| 2  | [What are the different data types in JavaScript](#2-what-are-the-different-data-types-in-javascript)  |
| 3  | [What are the different ways to create an Object in JavaScript](#3-what-are-the-different-ways-to-create-an-object-in-javascript)  |
| 4  | [Difference between == and === operators](#4-difference-between--and--operators)  |
| 5  | [Is javascript single-threaded or multi-threaded](#5-is-javascript-single-threaded-or-multi-threaded)  |
| 6  | [What are arrow functions and its features](#6-what-are-arrow-functions-and-its-features)  |
| 7  | [Explain passed by value and passed by reference](#7-explain-passed-by-value-and-passed-by-reference)  |
| 8  | [What do you mean by Synthetic events](#8-what-do-you-mean-by-synthetic-events)  |
| 9  | [What is Prototype and Prototype Inheritance](#9-what-is-prototype-and-prototype-inheritance)  |
| 10 | [What are callback functions](#10-what-are-callback-functions)  |
| 11 | [What is array destructuring](#11-what-is-array-destructuring)  |
| 12 | [What are promises](#12-what-are-promises)  |
| 13 | [Can we combine two arrays using any es6 operators](#13-can-we-combine-two-arrays-using-any-es6-operators)  |
| 14 | [Difference between let, var, const](#14-difference-between-let-var-const)  |
| 15 | [What is Closure](#15-what-is-closure)  |
| 16 | [What is Hoisting](#16-what-is-hoisting)  |
| 17 | [Difference between JSON and Object](#17-difference-between-json-and-object)  |
| 18 | [Difference between Map and filter](#18-difference-between-map-and-filter)  |
| 19 | [Difference between Call, apply, bind](#19-difference-between-call-apply-bind)  |

### 1. What is JavaScript
* JavaScript is the world's most popular programming language used for web development. It can be used to update HTML and CSS
* Nowadays, JavaScript is getting used in many other areas e.g. server-side development, mobile app development etc.

### 2. What are the different data types in JavaScript
| Primitive   |Non-primitive |
| ------------- | ------------- |
| Boolean, NULL, undefined, BigInt, String, Number, Symbol  | Object | 

### 3. What are the different ways to create an Object in JavaScript

##### a) Object Literals: A comma-separated set of name and value pairs that is wrapped inside curly braces.

```
var person = {
    name: 'Surbhi',
    age: 25,
    occupation: 'Software Engineer'
}
```
##### b) Object.create method: TCreates a new object, by using an existing object as the prototype of the newly created object.

```
const person = {
    name: 'Surbhi',
    age: 25,
    occupation: 'Software Engineer'
}

var info = Object.create(person);
console.log(info.name); // output - Surbhi

Here "person" is an existing object which is passed as a prototype to the newly created object "info"
```

##### c) Object constructor: Constructor function allows to create objects with the help of new keyword

```
const person = new Person();
```

##### d) using ES6: We can create object using ES6 class feature

```
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


### 7. Explain passed by value and passed by reference

### 8. What do you mean by Synthetic events

### 9. What is Prototype and Prototype Inheritance

### 10. What are callback functions

### 11. What is array destructuring

### 12. What are promises

### 13. Can we combine two arrays using any es6 operators
* Yes, using Spread Operators
```
const arr1 = [1,2,3,4];
const arr2 = [5,6];
const arr3 = [...arr1, ...arr2]
console.log(arr3) //output - [1,2,3,4,5,6]
```

### 14. Difference between let, var, const

### 15. What is Closure

### 16. What is Hoisting

### 17. Difference between JSON and Object

### 18. Difference between Map and filter

### 19. Difference between Call, apply, bind

******************************In progress


