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

## **Arrays**: 
Used to store collections of values. Arrays can contain elements of any data type.

   ```javascript
   let colors = ["red", "green", "blue"];
   let numbers = [1, 2, 3, 4, 5];
   ```
  Here are some "types" of arrays you might come across or create in JavaScript:

 -- **Single-Dimensional Arrays (One-dimensional arrays)**
   - These are the simplest form of arrays that represent a list of elements. You can access elements using a single index.
   ```javascript
   let fruits = ['apple', 'banana', 'cherry'];
   ```

 -- **Multi-Dimensional Arrays (Two-dimensional or more)**
   - These are arrays that contain one or more arrays as their elements, allowing you to create a matrix-like structure.
   ```javascript
   let matrix = [
     [1, 2, 3],
     [4, 5, 6],
     [7, 8, 9]
   ];
   ```

--  **Typed Arrays**
   - Typed arrays are a set of arrays that provide a mechanism for accessing raw binary data. These include `Int8Array`, `Uint8Array`, `Uint8ClampedArray`, `Int16Array`, `Uint16Array`, `Int32Array`, `Uint32Array`, `Float32Array`, and `Float64Array`.
   ```javascript
   let int16 = new Int16Array([1, 2, 3]);
   ```

 -- **Associative Arrays (Not officially supported as a type)**
   - While JavaScript doesn't have "associative arrays" like some other languages, you can use objects to create a similar construct, with key-value pairs.
   ```javascript
   let person = {
     firstName: "John",
     lastName: "Doe",
     age: 50
   };
   ```

 -- **Sparse Arrays**
   - Arrays that have not had values assigned to all of their indices, or where you have deleted elements, leaving "holes" in the index sequence.
   ```javascript
   let sparseArray = [1, , , 4]; // Index 1 and 2 are empty
   ```

 -- **Dense Arrays**
   - These are arrays where every index from 0 up to the `length - 1` has been assigned a value. There are no "holes" in the index sequence.
   ```javascript
   let denseArray = [1, 2, 3, 4]; // No empty indices
   ```

 -- **Parallel Arrays**
   - This concept involves maintaining two or more arrays of the same length where each array holds different attributes of a set of objects.
   ```javascript
   let names = ['John', 'Jane', 'Doe'];
   let ages = [25, 29, 22];
   // 'John' is 25, 'Jane' is 29, and 'Doe' is 22
   ```

   ** Commonly Used JavaScript Array Methods**

In JavaScript, arrays come with many built-in methods to perform various operations. Here's a list of some of the most commonly used array methods along with a brief description of what they do:

*  **`push()`** - Adds one or more elements to the end of an array and returns the new length of the array.
* **`pop()`** - Removes the last element from an array and returns that element.
* **`shift()`** - Removes the first element from an array and returns that element.
* **`unshift()`** - Adds one or more elements to the beginning of an array and returns the new length of the array.
* **`forEach()`** - Executes a provided function once for each array element.
* **`map()`** - Creates a new array with the results of calling a provided function on every element in the calling array.
* **`filter()`** - Creates a new array with all elements that pass the test implemented by the provided function.
* **`reduce()`** - Applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value.
* **`reduceRight()`** - Applies a function against an accumulator and each value of the array (from right-to-left) to reduce it to a single value.
* **`sort()`** - Sorts the elements of an array in place and returns the array. The default sort order is ascending, built upon converting the elements into                    strings and comparing their sequences of UTF-16 code units values.
*  **`reverse()`** - Reverses the order of the elements in an array in place — the first becomes the last, and the last becomes the first.
*  **`slice()`** - Returns a shallow copy of a portion of an array into a new array object selected from start to end (end not included) where start and end                      represent the index of items in that array.
*  **`splice()`** - Changes the contents of an array by removing or replacing existing elements and/or adding new elements in place.
*  **`join()`** - Joins all elements of an array into a string and returns this string.
*  **`concat()`** - Is used to merge two or more arrays, and returns a new array, without changing the existing arrays.
*  **`indexOf()`** - Returns the first index at which a given element can be found in the array, or -1 if it is not present.
*  **`lastIndexOf()`** - Returns the last index at which a given element can be found in the array, or -1 if it is not present.
*  **`includes()`** - Determines whether an array includes a certain value among its entries, returning true or false as appropriate.
*  **`find()`** - Returns the value of the first element in the array that satisfies the provided testing function.
*  **`findIndex()`** - Returns the index of the first element in the array that satisfies the provided testing function.
*  **`every()`** - Tests whether all elements in the array pass the test implemented by the provided function.
*  **`some()`** - Tests whether at least one element in the array passes the test implemented by the provided function.
*  **`Array.from()`** - Creates a new Array instance from an array-like or iterable object.
*  **`Array.of()`** - Creates a new Array instance with a variable number of arguments, regardless of number or type of the arguments.
*  **`flat()`** - Creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.
*  **`flatMap()`** - First maps each element using a mapping function, then flattens the result into a new array.

   Remember, each of these methods may alter the original array or create a new one, and they may take callback functions or specific parameters to perform       their tasks. It's important to understand these details to effectively use each method in your JavaScript code.


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
1. **if statement**
2. **if-else statement**
3. **if-else if-else statement**
4. **switch statement**
5. **ternary operator**

Let's dive into each one:

### 1. `if` statement
The `if` statement evaluates a condition. If the condition is `true`, the code inside the `if` block is executed.

```javascript
let age = 18;
if (age >= 18) {
    console.log("You are eligible to vote.");
}
```

### 2. `if-else` statement
The `if-else` statement evaluates a condition. If the condition is `true`, the code inside the `if` block is executed; otherwise, the code inside the `else` block is executed.

```javascript
let age = 16;
if (age >= 18) {
    console.log("You are eligible to vote.");
} else {
    console.log("You are not eligible to vote.");
}
```

### 3. `if-else if-else` statement
This is used when there are multiple conditions to evaluate. The conditions are checked from top to bottom. As soon as one condition is found to be `true`, the code inside that block is executed, and the rest of the conditions are skipped.

```javascript
let score = 85;
if (score >= 90) {
    console.log("Grade A");
} else if (score >= 80) {
    console.log("Grade B");
} else if (score >= 70) {
    console.log("Grade C");
} else {
    console.log("Grade D");
}
```

### 4. `switch` statement
The `switch` statement is used to perform different actions based on different conditions. It's especially useful when you have a single expression to evaluate against multiple possible values.

```javascript
let fruit = "apple";
switch (fruit) {
    case "banana":
        console.log("Yellow fruit");
        break;
    case "apple":
        console.log("Red or green fruit");
        break;
    case "orange":
        console.log("Orange fruit");
        break;
    default:
        console.log("Unknown fruit");
}
```

### 5. Ternary Operator
The ternary operator is a shorthand way of writing an `if-else` statement. It's particularly useful for short, simple conditions.

```javascript
let age = 18;
let eligibility = age >= 18 ? "eligible to vote" : "not eligible to vote";
console.log(eligibility);
```

In the above example, if `age` is 18 or more, "eligible to vote" is assigned to `eligibility`, otherwise "not eligible to vote" is assigned.

## Loops:
- Loops are used to execute a block of code repeatedly. JavaScript provides `for`, `while`, and `do...while` loops for different looping scenarios.
- Certainly! Here's an expanded explanation about loops in JavaScript, formatted as a Markdown text:

---

## Loops in JavaScript

Loops are fundamental constructs in programming that allow you to execute a block of code multiple times. JavaScript offers several types of loops for different scenarios:

### 1. `for` Loop
- **Usage:** Ideal when the number of iterations is known.
- **Syntax:**
  ```javascript
  for (initialization; condition; increment) {
      // code block to be executed
  }
  ```

### 2. `while` Loop
- **Usage:** Suitable when the number of iterations is not known in advance and depends on a conditional expression.
- **Syntax:**
  ```javascript
  while (condition) {
      // code block to be executed
  }
  ```

### 3. `do...while` Loop
- **Usage:** Similar to the `while` loop, but guarantees that the code block is executed at least once.
- **Syntax:**
  ```javascript
  do {
      // code block to be executed
  } while (condition);
  ```

### 4. `for...in` Loop
- **Usage:** Designed for iterating over the properties of an object.
- **Syntax:**
  ```javascript
  for (variable in object) {
      // code to execute for each property
  }
  ```

### 5. `for...of` Loop
- **Usage:** Introduced in ES6 for iterating over iterable objects like arrays, strings, maps, sets, etc.
- **Syntax:**
  ```javascript
  for (variable of iterable) {
      // code to execute for each element
  }
  ```

### Best Practices for Using Loops
- **Break and Continue:** Use `break` to exit a loop completely and `continue` to skip the current iteration and proceed to the next one.
- **Performance:** Be cautious with conditions in loops to avoid infinite loops which can crash your application.
- **Readability:** Choose the right type of loop for clarity and better understanding of the code.

Loops are a powerful feature in JavaScript, enabling efficient and concise code for tasks that require repetitive actions.


## Functions:

Functions are one of the fundamental building blocks in JavaScript. Here's an overview of various types of functions with simple examples:

## 1. Regular Functions

The most basic type of function.

```javascript
function greet(name) {
    return "Hello, " + name + "!";
}
console.log(greet("Alice")); // "Hello, Alice!"
```

## 2. Anonymous Functions

Functions that don't have a name.

```javascript
const greeting = function(name) {
    return "Hi, " + name + "!";
}
console.log(greeting("Bob")); // "Hi, Bob!"
```

## 3. Arrow Functions

A more concise syntax for writing function expressions.

```javascript
const greetArrow = (name) => "Hey, " + name + "!";
console.log(greetArrow("Charlie")); // "Hey, Charlie!"
```

## 4. Immediately Invoked Function Expressions (IIFE)

Functions that run as soon as they are defined.

```javascript
(function() {
    console.log("I am an IIFE!");
})();
```

## 5. Constructor Functions

Functions that are used to create objects.

```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
}

const person1 = new Person("Diana", 30);
console.log(person1.name); // "Diana"
```

## 6. Generator Functions

Functions that can be exited and later re-entered.

```javascript
function* idGenerator() {
    let id = 0;
    while (true) {
        yield id++;
    }
}

const gen = idGenerator();
console.log(gen.next().value); // 0
console.log(gen.next().value); // 1
```

## 7. Async Functions

Functions that return a promise, allowing the use of `await` within them.

```javascript
async function fetchData(url) {
    let response = await fetch(url);
    let data = await response.json();
    return data;
}

// fetchData('https://api.example.com/data').then(console.log);
```

## 8. Callback Functions

Functions passed as an argument to another function.

```javascript
function doSomething(callback) {
    // simulate some async operation
    setTimeout(function() {
        console.log("Task done!");
        callback();
    }, 1000);
}

doSomething(function() {
    console.log("Callback called!");
});
```

## Objects:
- Objects are complex data structures used to represent real-world entities. They consist of key-value pairs, where keys are unique identifiers for properties and values represent the data associated with those properties.

## Definition and Creation

In JavaScript, an object is an unordered collection of key-value pairs. The keys (or properties) can be strings or symbols, and the values can be anything from primitives to complex data types.

Objects can be created in several ways:

### Object Literals

The simplest way to create an object is using an object literal:

```javascript
let person = {
    name: "John Doe",
    age: 30,
    greet: function() {
        console.log("Hello!");
    }
};
```

### Constructor Functions

You can also create objects using constructor functions:

```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
    this.greet = function() {
        console.log("Hello!");
    };
}

let person = new Person("John Doe", 30);
```

### `Object.create()`

Another method is `Object.create()`, which creates a new object with the specified prototype object:

```javascript
let proto = {
    greet: function() {
        console.log("Hello!");
    }
};

let person = Object.create(proto);
person.name = "John Doe";
person.age = 30;
```

## Properties and Methods

### Accessing Properties

You can access properties using dot notation or bracket notation:

```javascript
console.log(person.name); // "John Doe"
console.log(person['age']); // 30
```

### Adding and Modifying Properties

Adding or modifying properties is straightforward:

```javascript
person.gender = "male";
person.greet = function() {
    console.log("Hi, I'm " + this.name);
};
```

### Deleting Properties

Properties can be removed using the `delete` keyword:

```javascript
delete person.age;
```

## Prototypes

Every JavaScript object has a prototype, which is another object from which it inherits properties.

```javascript
let parent = {
    sayHello: function() {
        console.log("Hello from parent");
    }
};

let child = Object.create(parent);
child.sayHello(); // "Hello from parent"
```

## Scope and Closures:
- Scope refers to the visibility and accessibility of variables in different parts of your code. Closures are functions that "remember" the scope in which they were created, even when executed outside that scope.

## Callbacks and Higher-Order Functions:
- Callbacks are functions passed as arguments to other functions and are called after a specific task is completed. Higher-order functions are functions that take other functions as arguments or return them.

## Callback Syntax 

 ```javascript
  functionA(function(error, resultA) {
    if (error) {
        // handle error
    } else {
        functionB(resultA, function(error, resultB) {
            if (error) {
                // handle error
            } else {
                functionC(resultB, function(error, resultC) {
                    // ... and so on
                });
            }
        });
    }
});
```

## Syntax of Promises Chaining:

```javascript
functionA()
    .then(resultA => functionB(resultA))
    .then(resultB => functionC(resultB))
    .catch(error => {
        // handle any error that occurred in any of the previous steps
    });
```

## Asynchronous JavaScript:
- Asynchronous JavaScript allows non-blocking execution of code, enabling operations like making HTTP requests or handling time-consuming tasks without freezing the user interface.

## DOM Manipulation:
- The Document Object Model (DOM) represents the structure of a web page. JavaScript can interact with the DOM to dynamically change HTML elements and their attributes. This includes altering content, changing styles, adding or removing elements, and handling events. Below are some common operations in DOM manipulation:

| Operation                  | Syntax                                                                                        | Description                                    |
|----------------------------|-----------------------------------------------------------------------------------------------|------------------------------------------------|
| *Selecting Elements*     |                                                                                               |                                                |
| By ID                      | `document.getElementById('elementId')`                                                        | Selects a single element by its ID.            |
| By Class                   | `document.getElementsByClassName('className')`                                                | Selects all elements with the specified class. |
| By Tag                     | `document.getElementsByTagName('tagName')`                                                    | Selects all elements with the specified tag.   |
| Query Selector             | `document.querySelector('.className')` or `document.querySelector('#elementId')`              | Selects the first element matching the query.  |
| *Modifying Content*      |                                                                                               |                                                |
| Changing Text              | `document.getElementById('elementId').innerText = 'New Text';`                                | Changes the text content of an element.        |
| Changing HTML              | `document.getElementById('elementId').innerHTML = '<b>New HTML</b>';`                         | Changes the HTML content of an element.        |
| **Changing Styles**        |                                                                                               |                                                |
| Modifying Styles           | `document.getElementById('elementId').style.color = 'red';`                                   | Alters the style of an element.                |
| **Creating & Adding Elements** |                                                                                             |                                                |
| Creating a New Element     | `var newDiv = document.createElement('div');`                                                 | Creates a new HTML element.                    |
| Adding Text to Element     | `newDiv.innerText = 'Hello World';`                                                           | Adds text to a newly created element.          |
| Appending to the DOM       | `document.body.appendChild(newDiv);`                                                          | Adds the new element to the DOM.               |
| **Removing Elements**      |                                                                                               |                                                |
| Remove an Element          | `var elementToRemove = document.getElementById('elementId'); elementToRemove.parentNode.removeChild(elementToRemove);` | Removes an element from the DOM.               |
| *Event Handling*         |                                                                                               |                                                |
| Adding an Event Listener   | `document.getElementById('elementId').addEventListener('click', function() { alert('Element clicked!'); });` | Adds an event listener to an element.          |
| *Changing Attributes*   |                                                                                               |                                                |
| Set Attribute              | `document.getElementById('elementId').setAttribute('href', 'https://example.com');`           | Sets an attribute of an element.               |
| Get Attribute              | `var attributeValue = document.getElementById('elementId').getAttribute('href');`             | Retrieves an attribute value of an element.    |
| *Class Manipulation*     |                                                                                               |                                                |
| Add a Class                | `document.getElementById('elementId').classList.add('newClass');`                             | Adds a class to an element.                    |
| Remove a Class             | `document.getElementById('elementId').classList.remove('existingClass');`                     | Removes a class from an element.               |
| Toggle a Class             | `document.getElementById('elementId').classList.toggle('activeClass');`                       | Toggles a class on an element.                 |


  

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
  
# JavaScript Regular Expressions

Regular expressions in JavaScript are patterns used to match character combinations in strings. They are an extremely powerful tool for searching and manipulating text. Here's a brief overview of how to use regular expressions (regex) in JavaScript:

## Creating a Regular Expression
There are two ways to create a regex in JavaScript:

1. **Literal Notation**: Using two forward slashes (`/`) with the pattern in between.
   ```javascript
   let re = /pattern/;
   ```

2. **Constructor Function of the `RegExp` Object**:
   ```javascript
   let re = new RegExp('pattern');
   ```

## Flags
Regular expressions can have flags that affect the search. Common flags include:

- `g`: Global search (find all matches rather than stopping after the first match)
- `i`: Case-insensitive search
- `m`: Multi-line search

Example with flags:
```javascript
let re = /pattern/gi;
```

## Methods Using Regex
- **test()**: Checks if a pattern exists in a string. Returns `true` or `false`.
  ```javascript
  re.test('string to test');
  ```

- **exec()**: Finds a match in a string. Returns an array of information or `null`.
  ```javascript
  re.exec('string to test');
  ```

- **match()**: Applied to a string and returns an array of matches.
  ```javascript
  'string to test'.match(re);
  ```

- **replace()**: Replaces matches in a string with a new substring.
  ```javascript
  'string to test'.replace(re, 'newSubstr');
  ```

- **search()**: Tests for a match in a string. Returns the index of the match, or `-1` if the search fails.
  ```javascript
  'string to test'.search(re);
  ```

- **split()**: Uses a regex or a fixed string to break a string into an array of substrings.
  ```javascript
  'string to test'.split(re);
  ```

## Example Pattern
A simple pattern to match an email address might look like this:
```javascript
let emailPattern = /\S+@\S+\.\S+/;
```



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
- **AJAX** stands for **Asynchronous JavaScript and XML**.
- It allows web pages to update asynchronously by exchanging data with a web server.
- AJAX can send and receive data in the background, without refreshing the page.

## Why Use AJAX?
- Provides a **faster user experience** by updating parts of a page.
- Reduces **server load** and **bandwidth**.
- Allows web pages to be **dynamic and interactive**.

## Key Concepts
1. **XMLHttpRequest Object:** Central to AJAX for server communication.
2. **JavaScript:** Used for handling data and manipulating the DOM.
3. **JSON:** Common data format for AJAX communication.

## How AJAX Works
1. An event on the web page triggers an AJAX call.
2. JavaScript creates an `XMLHttpRequest` object.
3. The object sends a request to the server.
4. The server processes the request.
5. The server sends a response back.
6. JavaScript processes the response and updates the page.

## Simple AJAX Example
```javascript
// Create XMLHttpRequest object
var xhttp = new XMLHttpRequest();

// Define the response handler
xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    console.log(this.responseText);
  }
};

// Open the request
xhttp.open("GET", "url-to-fetch-data-from", true);

// Send the request
xhttp.send();
```

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

