# JS Cheat Sheet

## What is JavaScript?
JavaScript is a Synchronous, Single Threaded Programming language.

## Variables:
Variables are used to store and manage data values in programming languages. In JavaScript, you can declare variables using the `let`, `const`, or `var` keywords. The `let` and `const` keywords were introduced in newer versions of JavaScript (ES6), while `var` has been used in older versions. Here, I'll focus on `let` and `const`.

1. **`let`**: Variables declared with `let` can be reassigned to new values after they're initially assigned. They have block scope, meaning they're only accessible within the block of code they're declared in.

   ```javascript
   let age = 25;
   age = 26; // Valid, reassigning the value
   ```

2. **`var`**: Variables declared with `var`, is an older version of declaring variables. It doesn't have a block scope, meaning it can be declared and accessed entire program.

   ```javascript
   var age = 17;
   age = 30; // Valid, reassigning the value
   ```

3.  **`const`**: Variables declared with `const` are used for values that won't change after they're assigned. They also have a block scope. Once assigned, their value cannot be changed or reassigned.

   ```javascript
   const pi = 3.14159;
   // pi = 3.14; // Error, cannot reassign a constant
   ```

### Data Types:
JavaScript has several built-in data types that determine the kind of values that can be stored in variables. Here are some of the fundamental data types:

1. **Numbers**: Used for numeric values, including integers and floating-point numbers.

   ```javascript
   let age = 25; // Integer
   let price = 19.99; // Floating-point number
   ```

2. **Strings**: Used for textual data. Strings are enclosed in single or double quotes.

   ```javascript
   let name = "John";
   let message = 'Hello, world!';
   ```

3. **Booleans**: Used for representing true or false values.

   ```javascript
   let isStudent = true;
   let hasCar = false;
   ```

4. **Arrays**: Used to store collections of values. Arrays can contain elements of any data type.

   ```javascript
   let colors = ["red", "green", "blue"];
   let numbers = [1, 2, 3, 4, 5];
   ```

5. **Objects**: Used to store key-value pairs, where each key is a string (or symbol) and each value can be of any data type.

   ```javascript
   let person = {
       firstName: "John",
       lastName: "Doe",
       age: 30,
       isStudent: false
   };
   ```

6. **Null**: Represents the intentional absence of any value or object.

   ```javascript
   let emptyValue = null;
   ```

7. **Undefined**: Represents an uninitialized or unassigned value.

   ```javascript
   let undefinedValue;
   ```

## Operators:
- Operators are symbols used to perform operations on variables and values. JavaScript includes arithmetic, assignment, comparison, and logical operators to perform various tasks.

## Conditional Statements:
- Conditional statements like `if`, `else`, `else if`, and `switch` allow you to make decisions in your code based on certain conditions.

## Loops:
- Loops are used to execute a block of code repeatedly. JavaScript provides `for`, `while`, and `do...while` loops for different looping scenarios.

## Functions:
- Functions are blocks of code designed to perform a specific task. They are reusable and can take arguments and return values.

## Arrays:
- Arrays are used to store multiple values in a single variable. Each value is indexed, starting from 0, allowing easy access and manipulation of the data.

## Objects:
- Objects are complex data structures used to represent real-world entities. They consist of key-value pairs, where keys are unique identifiers for properties and values represent the data associated with those properties.

## Scope and Closures:
- Scope refers to the visibility and accessibility of variables in different parts of your code. Closures are functions that "remember" the scope in which they were created, even when executed outside that scope.

## Callbacks and Higher-Order Functions:
- Callbacks are functions passed as arguments to other functions and are called after a specific task is completed. Higher-order functions are functions that take other functions as arguments or return them.

## Asynchronous JavaScript:
- Asynchronous JavaScript allows non-blocking execution of code, enabling operations like making HTTP requests or handling time-consuming tasks without freezing the user interface.

## DOM Manipulation:
- The Document Object Model (DOM) represents the structure of a web page. JavaScript can interact with the DOM to dynamically change HTML elements and their attributes.

## Events and Event Listeners:
- Events are actions that occur on a web page, like clicks or keypresses. Event listeners are used to "listen" for these events and execute specific actions when triggered.

## JSON:
- JSON (JavaScript Object Notation) is a lightweight data-interchange format that is easy to read and write. It is commonly used for data exchange between a server and a web application.

## ES6 Features:
- ES6 (ECMAScript 2015) introduced several new features to JavaScript, such as let, const, arrow functions, template literals, destructuring, and more.

## Classes and Prototypes:
- ES6 classes provide a syntax for creating object blueprints with constructor functions and prototype-based inheritance.

## Modules:
- ES6 Modules allow organizing code into separate files and exporting/importing functionality between them.

## Fetch API:
- The Fetch API is used to make HTTP requests and handle responses asynchronously.

## Error Handling:
- Error handling is a way to gracefully handle errors in JavaScript using try...catch blocks.

## Regular Expressions:
- Regular expressions (RegExp) are used for pattern matching and text searching.

## Built-in Objects:
- JavaScript provides several built-in objects like Math, Date, Array, String, and more, offering various utility methods and properties.

## Document Object Model (DOM) Traversal and Manipulation:
- DOM traversal and manipulation allow selecting specific elements on a web page and modifying their content, styles, and attributes dynamically.

## Local Storage and Session Storage:
- Local Storage and Session Storage are Web Storage APIs used to store data locally in a web browser.

## Web APIs:
- Web APIs are browser-provided interfaces that allow access to various functionalities, such as geolocation, WebSockets, and more.

## Scope and Hoisting:
- Scope refers to the context in which variables are declared and accessible. Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their scope during the compilation phase.

## Strict Mode:
- Strict mode is a feature in JavaScript that enforces a stricter set of rules for writing code, reducing certain errors and improving code quality.

## Event Bubbling and Event Capturing:
- Event propagation in the DOM can happen through event bubbling (events trigger on the target element and propagate up the DOM tree) or event capturing (events trigger on the outermost ancestor and propagate down the DOM tree).

## AJAX:
- AJAX (Asynchronous JavaScript and XML) is a technique used to send and retrieve data from the server asynchronously without refreshing the entire web page.

## Callback Hell and Promises Chaining:
- Callback hell occurs when multiple nested callbacks lead to complex and unreadable code. Promises chaining is a way to simplify asynchronous operations and avoid callback hell.

## Set, Map, WeakSet, WeakMap:
- These data structures provide unique collections and support weak references, which can be useful for memory management and specialized use cases.

## Functional Programming Concepts:
- Functional programming concepts involve using higher-order functions like map, filter, and reduce to process data in a functional and declarative manner.

## Prototypal Inheritance and Object.create():
- Prototypal inheritance is a way to share properties and methods between objects. The `Object.create()` method is used to create new objects with a specified prototype.

## Call, Apply, and Bind Methods:
- These methods are used to set the value of `this` in a function when calling it.

## this Keyword:
- The `this` keyword refers to the object on which a method is called, and its value changes depending on how the method is called.

## Destructuring Assignment:
- Destructuring allows extracting values from arrays or properties from objects into separate variables.

## Context vs. Scope:
- Context and scope are related but different concepts in JavaScript. Context refers to the value of `this` within a function, while scope refers to the accessibility of variables.

## Memory Management and Garbage Collection:
- JavaScript uses automatic memory management to handle memory allocation and deallocation. Garbage collection is the process of freeing up memory occupied by objects that are no longer in use.

## Throttling and Debouncing:
- Throttling and debouncing are techniques used to control the rate of function execution in response to frequent events like scrolling or resizing.

## WebSockets and Real-Time Communication:
- WebSockets enable real-time communication between a client and a server, allowing bidirectional data transfer.

## Generators and Iterators:
- Generators allow writing functions that can be paused and resumed, while iterators are objects used to traverse data structures.

## Async Iteration and Iterables:
- Async iterators allow asynchronous traversal of data structures using the `for-await-of` loop.

## Web Workers:
- Web Workers allow running JavaScript code in the background, separate from the main execution thread, for better performance and responsiveness.

## Proxy and Reflection API:
- Proxies provide a way to intercept and customize operations on objects, while the Reflection API allows inspecting and manipulating objects at runtime.
---

