# javascript
## Datatype

In JavaScript, a data type refers to the classification of values that variables can hold. JavaScript has several built-in data types, which can be categorized as primitive and non-primitive data types.

### Primitive Data Types:

Number: Represents numeric values, such as integers and floating-point numbers.

String: Represents sequences of characters enclosed in single or double quotes.

Boolean: Represents a logical value of either true or false.

Null: Represents the intentional absence of any object value.

Undefined: Represents a variable that has been declared but has not been assigned a value.

Symbol: Represents a unique identifier and is used in advanced JavaScript scenarios.

Primitive data types in JavaScript are immutable, which means their values cannot be changed once assigned. When you perform operations on primitive values, a new value is created rather than modifying the original value.

let age = 25;               // Number

let name = "John Doe";      // String

let isStudent = true;       // Boolean

let score = null;           // Null

let x;                      // Undefined

console.log(typeof age);    // Output: "number"

console.log(typeof name);   // Output: "string"

console.log(typeof isStudent);  // Output: "boolean"

console.log(typeof score);  // Output: "object"

console.log(typeof x);      // Output: "undefined"

### Non-Primitive Data Types:

Object: Represents a collection of key-value pairs or properties. Objects can contain functions, arrays, and other objects.

Array: Represents an ordered collection of values enclosed in square brackets.

Function: Represents a reusable block of code that performs a specific task.

Non-primitive data types in JavaScript are mutable, meaning their values can be modified directly.

let person = {              // Object

name: "John Doe",

age: 25,

isStudent: true

};

let numbers = [1, 2, 3, 4, 5];  // Array

function greet() {          // Function

console.log("Hello!");

}

console.log(typeof person);  // Output: "object"

console.log(typeof numbers); // Output: "object"

console.log(typeof greet);   // Output: "function"

variable:

In JavaScript, a variable is a named container used to store data values. Variables allow you to store and manipulate data in your programs. You can assign values to variables and retrieve those values later in your code.

To declare a variable in JavaScript, you can use the var, let, or const keyword followed by the variable name. Here's the general syntax:

var variableName;

let variableName;

const variableName;

The var keyword was traditionally used to declare variables in JavaScript. Variables declared with var are function-scoped or globally scoped, depending on where they are declared. However, var has some behavior quirks, such as variable hoisting and lack of block scope, so it's generally recommended to use let or const instead.

The let keyword was introduced in ECMAScript 6 (ES6) and provides block scope. Variables declared with let are limited to the block in which they are defined, such as within a function or a loop.

The const keyword is also introduced in ES6 and is used to declare constants, which are variables that cannot be reassigned once a value is assigned to them. Like let, const is also block-scoped.

Here are some examples of variable declarations and assignments:

let age;              // Variable declaration

age = 25;             // Variable assignment

let name = "John";    // Variable declaration and assignment in one line

const PI = 3.14159;   // Constant declaration and assignment

var count = 10;       // Legacy syntax for variable declaration and assignment

Variables can hold different types of data, such as numbers, strings, booleans, objects, arrays, or functions. The data type of a variable is determined by the value assigned to it, and it can be changed by assigning a new value of a different type to the variable.

It's important to note that JavaScript is a dynamically typed language, which means you don't need to explicitly declare the data type of a variable. The data type is automatically inferred based on the assigned value.

function

in JavaScript, a function is a block of reusable code that performs a specific task or calculates a value. Functions are a fundamental building block in JavaScript programming and are used to organize and modularize code.

A function in JavaScript can be defined using the function keyword, followed by the function name, a pair of parentheses (), and a block of code enclosed in curly braces {}

function addNumbers(num1, num2) {

let sum = num1 + num2;

return sum;

}

Functions in JavaScript can also be assigned to variables, passed as arguments to other functions, or even defined inside other functions (nested functions). JavaScript functions are highly flexible and powerful, enabling you to write complex and reusable code.

operator

In JavaScript, operators are symbols or keywords that perform operations on values, variables, or expressions. They allow you to manipulate and combine data in various ways. JavaScript includes a wide range of operators for different purposes, including arithmetic, assignment, comparison, logical, and more. Here are some commonly used operators in JavaScript:

Arithmetic Operators:

Addition: +

Subtraction: ``

Multiplication: ``

Division: /

Modulo (remainder): %

Increment: ++

Decrement: -

Assignment Operators:

Assignment: =

Addition assignment: +=

Subtraction assignment: =

Multiplication assignment: =

Division assignment: /=

Modulo assignment: %=

Comparison Operators:

Equal to: ==

Not equal to: !=

Strict equal to: ===

Strict not equal to: !==

Greater than: >

Less than: <

Greater than or equal to: >=

Less than or equal to: <=

Logical Operators:

Logical AND: &&

Logical OR: ||

Logical NOT: !

String Operators:

Concatenation: +

Conditional (Ternary) Operator:

Syntax: condition ? value1 : value2

Type Operators:

typeof: Returns the type of a value or variable as a string.

instanceof: Checks if an object belongs to a specific class or constructor.

These are just some of the basic operators in JavaScript. There are also bitwise operators, assignment operators with bitwise operations, and more. Operators can be used in combination with variables, literals, or expressions to perform calculations, comparisons, and logical operations.

data structure:

In JavaScript, data structures are used to store, organize, and manipulate data in a structured and efficient manner. JavaScript provides several built-in data structures that you can use to handle different types of data and perform various operations. Here are some commonly used data structures in JavaScript:

Array: An array is an ordered collection of values, accessed using numeric indices. It can store any type of data, including numbers, strings, objects, and even other arrays. Arrays in JavaScript are dynamic and can grow or shrink in size as needed.

Example:

let numbers = [1, 2, 3, 4, 5];

let fruits = ['apple', 'banana', 'orange'];

Object: An object is an unordered collection of key-value pairs, where each value is associated with a unique key. Objects are useful for representing entities or complex data structures. Keys in an object can be strings or symbols.

Example:

let person = {

name: 'John',

age: 25,

profession: 'Engineer'

};

Map: The Map data structure allows you to store key-value pairs, similar to objects. However, unlike objects, the keys in a Map can be of any data type, and the order of elements is preserved. Maps also provide various methods for working with key-value pairs.

Example:

let map = new Map();

map.set('name', 'John');

map.set('age', 25);

map.set('profession', 'Engineer');

Set: The Set data structure allows you to store unique values of any type. It ensures that duplicate values are not allowed, so each value in a Set is unique. Sets also provide methods for performing set operations like union, intersection, and difference.

Example:

let set = new Set();

set.add(1);

set.add(2);

set.add(3);

Stack: A stack is a data structure that follows the Last-In-First-Out (LIFO) principle. Elements are added and removed from the top of the stack. JavaScript arrays can be used as a stack by using push() to add elements and pop() to remove elements.

Example:

let stack = [];

stack.push(1);

stack.push(2);

stack.push(3);

let topElement = stack.pop();

Queue: A queue is a data structure that follows the First-In-First-Out (FIFO) principle. Elements are added to the end of the queue and removed from the front. JavaScript arrays can be used as a queue by using push() to add elements and shift() to remove elements.

Example:

let queue = [];

queue.push(1);

queue.push(2);

queue.push(3);

let frontElement = queue.shift();

These are just a few examples of data structures available in JavaScript. Depending on your specific needs, you can also implement other data structures like linked lists, trees, graphs, and more using JavaScript objects and arrays. Additionally, libraries and frameworks in JavaScript often provide their own specialized data structures to optimize specific operations or solve particular problems.

control loop statement:

JavaScript provides several control loop statements that allow you to repeatedly execute a block of code under specific conditions. The following are the main loop statements in JavaScript:

for loop: The for loop is used to iterate a block of code a specific number of times. It consists of three parts: initialization, condition, and iteration.

Example:

for (let i = 0; i < 5; i++) {

console.log(i);

}

while loop: The while loop repeatedly executes a block of code as long as a specified condition is true. It checks the condition before each iteration.

Example:

let i = 0;

while (i < 5) {

console.log(i);

i++;

}

do-while loop: The do-while loop is similar to the while loop, but it checks the condition after each iteration. This guarantees that the code inside the loop executes at least once.

Example:

let i = 0;

do {

console.log(i);

i++;

} while (i < 5);

for...in loop: The for...in loop is used to iterate over the properties of an object. It executes the code block for each enumerable property in the object.

Example:

const person = {

name: 'John',

age: 25,

profession: 'Engineer'

};

for (let key in person) {

console.log(key + ': ' + person[key]);

}

for...of loop: The for...of loop is introduced in ECMAScript 6 and is used to iterate over iterable objects such as arrays, strings, and other iterable data structures.

Example:

const numbers = [1, 2, 3, 4, 5];

for (let number of numbers) {

console.log(number);

}

These loop statements allow you to control the flow of your code execution and perform repetitive tasks efficiently. Depending on your specific requirements, you can choose the appropriate loop statement to achieve the desired outcome.

class and object :

In JavaScript, classes and objects are used to implement object-oriented programming (OOP) concepts. Here's an overview of classes and objects in JavaScript:

Classes: A class is a blueprint for creating objects with similar properties and methods. It defines the structure and behavior of objects. In JavaScript, classes were introduced in ECMAScript 6 (ES6) to provide a more convenient way to define objects and their behaviors.

Example:

class Person {

constructor(name, age) {

this.name = name;

this.age = age;

}

sayHello() {

console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);

}

}

// Creating objects from the class

const person1 = new Person('John', 25);

const person2 = new Person('Jane', 30);

person1.sayHello(); // Output: Hello, my name is John and I am 25 years old.

person2.sayHello(); // Output: Hello, my name is Jane and I am 30 years old.

Objects: An object is an instance of a class. It represents a specific entity with its own set of properties and methods. Objects are created from a class using the new keyword. They can have their own unique values for properties defined in the class.

Example:

// Using the Person class from the previous example

const person1 = new Person('John', 25);

const person2 = new Person('Jane', 30);

console.log(person1.name); // Output: John

console.log(person2.age); // Output: 30

person1.sayHello(); // Output: Hello, my name is John and I am 25 years old.

person2.sayHello(); // Output: Hello, my name is Jane and I am 30 years old.

Objects allow you to create and work with instances of classes, providing a way to organize and structure your code based on the principles of object-oriented programming.
