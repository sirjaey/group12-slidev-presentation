---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://shorturl.at/C86WK
# some information about your slides (markdown enabled)
title: Group 12 Presentation
description: |
  This is a presentation for the group 12 project of the Altschool Tinyuka Frontend Engineering program.
  The presentation covers the project details, team members, and other relevant information.
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)

# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
# seoMeta:
#  ogImage: https://cover.sli.dev
---

# GROUP 12 PRESENTATION

AltSchool Tinyuka 2024/2025 Frontend Engineering

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/sirjaey/Group12-Slidev-Project" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# Meet the team

- Joshua Abu
- Adegbite Raheem
- Ugomma Esosa EzeOgali
- Isaiah Ayomide Yenou
- Ude Maduabuchi Onyedikachi
- Opeyemi Kolurejo
- Victoria Anthony
- Okedinachi Pleasant Chukwuderah
- Chumaraoke Daniel Njoku
- Olafare Temitope
- Stephanie Ayomide Adetomiwa 
<br>
<br>

<style>
h1 {
  background-color:rgb(52, 182, 43);
  background-image: linear-gradient(45deg, #4EC5D4 10%,rgb(16, 207, 73) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
transition: slide-up
level: 2
---

# Project Overview
-
-
-
-
-
-
-
-
-

<style>
h1 {
  background-color:rgb(52, 182, 43);
  background-image: linear-gradient(45deg, #4EC5D4 10%,rgb(16, 207, 73) 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>
---
transition: slide-up
level: 2
layout: center
---

# Data Types

---
level: 2
---

# Overview

- Data Types
- Operationals
- Conditionals
- Interaction
- Loops

---

# Data Types
<br>


 **What are Data Types:**
 Data types represent the different kinds of values you can work with in JavaScript. They tell the interpreter what kind of data is being stored or manipulated.

**Primary data types in JavaScript**
- String: Used to represent text enclosed in quotes.
- Number: This is used for both integers and decimals.
- Boolean: true or false.
- Null: Represents an Empty or unknown value.
- Undefined: A declared variable with no value.
- Object:A collection of key-value pairs.
- Array: A list of values.


---
layout: center
---

# Data Types Examples
```js
let name = "Ugomma";        // String
let age = 25;               // Number
let isStudent = true;       // Boolean
let empty = null;           // Null
let notSet;                 // Undefined
let person = {name: "Ama", age: 22}; // Object
let colors = ["red", "blue"];        // Array
```

---

# Operators

**What are Operators**
  Operators are symbols used to perform operations on values and variables, like arithmetic, comparison, and logical evaluations.

**Types of Operators**
- **Arithmetic Operators**:Used for mathematical operations (+, -, *, /, %).
- **Assignment Operators**:Used to assign values (=, +=, -=).
- **Comparison Operators**:Used to compare values (==, ===, !=, <, >).
- **Logical Operators**:Used to combine boolean expressions ( &&, ||, !).

---

# How to use operators

```js
//Arithmetic operators
let a = 10, b = 3;
a + b // 13
a - b // 7
a * b // 30
a / b // 3.33
a % b // 1 (remainder)
```


```js 
// Assignment Operators
 let x = 5; //basic assignment
 x += 2; //x = x + 2
 a -= 3; //a = a - 3
```

---


```js
//Comparison Operators
a == "10";   // true (equality)
a === "10";  // false (strict equality)
a != b;      // true
a > b;       // true
a < b;       // true
a >= b;      // true
a <= b;      // true

```


```js 
// Logical Operators
 true && false // false
true || false // true
!true         // false
```

---

# Conditionals
**What are conditionals**
Conditionals are used to execute different blocks of code based on certain conditions. This allows your program to make decisions.

**Types of conditionals**
- if else
- else if
- Ternary Operator(shorthand if..else)
---

**Types of conditionals**

**if...else**
```js
let score = 80;
if (score >= 70) {
  console.log("You passed!");
} else {
  console.log("Try again.");
}
```

**else if**
```js
let score = 80;
if (score >= 70) {
  console.log("You passed!");
} else {
  console.log("Try again.");
}
```

**Ternary Operator(shorthand if..else)**
```js
let result = score >= 70 ? "Passed" : "Failed";
console.log(result);
````
---

# Interaction

**What is interaction in Js?**
Interaction allows JavaScript to communicate with the user or developer through pop-ups or the console.

**Types of Interactions**

- alert(): Displays a simple message.
```js
alert("Welcome to my website!");
```

- console.log(): Outputs information to the browser's developer console.
```js
console.log("This is group 12's presentation");
```

- prompt(): Asks the user for input and returns it as a string.
```js
let name = prompt("What is your name?");
console.log("Hello, " + name);
```
---

# Loops
**What are Loops**
Loops are used to run the same block of code repeatedly, as long as a condition is true. They're useful for tasks like iterating through arrays or repeating actions.

**Types of Loops in JS**
- For Loop: This works best when you know how many times to loop.
```js
for (let i = 1; i <= 3; i++) {
  console.log("Count: " + i);
}
```
- While Loop:This is used when the number of iterations is unknown, but depends on a condition.
```js
let i = 1;
while (i <= 3) {
  console.log("While Count: " + i);
  i++;
}
```
- Do...While Loop: This is similar to while loop, but runs atleast once even if the condition is false.
```js
let j = 1;
do {
  console.log("Do Count: " + j);
  j++;
} while (j <= 3);
```
---
layout: center
---

# Functions in JavaScript
---

# Function Declaration
A Function declaration is a way to define a named function.

```javascript
function sayHello() {
  console.log("Hello Everybody"); //output: Hello Everybody
}
```
```javascript
function displayDetails (name, sex, age) {    
  console.log(`${name} is ${sex} and is ${age} years old`) // Output: John is male and is 25 years old
}
```
<br>

# Function Expression

This is another way to create a function and unlike function declaration it can be anonymous

```javascript
let displayDetails = function (name, sex, age) {
  console.log(`${name} is ${sex} and is ${age} years old`)
}
displayDetails("John", "male", 25)
```
```text
Output: John is male and is 25 years old
```
---

# Arrow Functions
Arrow functions provide a shorter way to write functions.

```javascript
  let displayDetails = () => {
   console.log(`${name} is ${sex} and is ${age} years old`) //Output = John is male and is 25 years old
  }
```

---

# Rest Parameters and Spread Syntax
The rest parameter allows you to represent an indefinite number of arguments as an array within a function and there can only be one rest parameter in a function's parameter list, and it must be the last parameter.

```javascript
function myFunc(a, b, ...restOfArgs) {
  console.log("First argument:", a);
  console.log("Second argument:", b);
  console.log("Rest of the arguments:", restOfArgs);
}
myFunc(1, 2, 3, 4, 5);// a = 1, b = 2, restOfArgs = 3,4,5
```
<br>
<h2>Spread Syntax</h2>
The spread syntax essentially unpacks an iterable (like a string or array).<br>
Spreads can be used to combine an array, clone an array and even spread a string into individual characters 

<div style = "display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 20px;">

```javascript

//combine array
let num1 = [1,2,3]
let num2 = [4,5,6]
const join = [...num1, ...num2]
```
```javascript

//clone array
let first = [9,8,7]

let second = [...first]
```
```javascript
//spread a string into individual characters
let string = "hey"

alert([...string])
```
</div>
---

# Closure and Variable Scope

<p>A closure is the ability of a function to "remember" and access variables from its outer scope, even after that function has finished executing. There are primarily two types of scope we're concerned with in this context:</p>
<ul>
<li>Global Scope: Variables declared outside of any function have global scope. They can be accessed from anywhere in your code.</li>
<li>Local Scope: Variables declared inside a function have local scope, they are only accessible within that function and any functions nested inside it. Also variables declared in a block of code has local scope.</li>
</ul>

```javascript
let globalVariable = "Accessible anywhere in code"

let localFunction = function() {
  let localVariable= "accessible only inside the function"
}
console.log(localVariable) // Error, not defined

```


---

# Function Object
<p>Functions being an object have properties like name, length.</p>
Accessing the "name" property of functions

```javascript
  let alpha = function beta() {
    alert("hey")
  }
console.log(alpha.name) // Output: beta

let sayHi = () => {
  console.log("hi")}
alert(sayHi.name) // Output = "sayHi" which is the contextual name Js got from the variable name
```

Accessing the "length" Property

```javascript
function rest (n, ...arr) {}
console.log(rest.length) // output = 1 because rest parameters aren't counted

function defaultValue(m, n=2, o, p){}
console.log(defaultValue.length) // Output = 1 because only m is counted before the default value

function destructure ({m,n}, o) {}
console.log(destructure.length) // output = 2 because the destructuring pattern counts as 1 parameter
```

---

# Scheduling
<p>Scheduling in JavaScript refers to the execution of code at specific points in time or in response to certain events.</p>
SetTimeout Method

```javascript
// setTimeout(function, delay);
let timeoutId = setTimeout((name) => {
  console.log(`Hello, ${name}!`);
}, 3000, "Chinedu");// 3000 meaning 3 secs represents the delay so the function will run after 3 secomds

// if we want to cancel or stop the function from executing, we use clearTimeOut method
clearTimeout(timeoutId); // The function won't run
```

---

# Using "func.call"
<p>In JS, func.call is a built-in JavaScript method that allows you to invoke a function with a specific this value and individual arguments passed directly. It is similar to func.apply()</p>

```javascript
const person = {
  name: "Chinedu",
  greet: function(greeting) {
    console.log(`${greeting}, my name is ${this.name}.`);
  }
};

const anotherPerson = {
  name: "Ifeoma"
};

person.greet.call(anotherPerson, "Hello"); // 'this' inside greet will refer to anotherPerson
// Output: Hello, my name is Ifeoma.
```

---
layout: center
---

# Objects in Javascript
---

<p>An object is a collection of key-value pairs, where each key (a string or Symbol) uniquely identifies a value (any JavaScript data type). Objects are fundamental for organizing and structuring data, representing entities, and building complex data structures in JavaScript. <br>
Object properties can be accessed using dot or square bracket notation.
</p>
An object can be created using the following Syntaxes:

```javascript
//object literal
let person = {}

//object constructor
let person = new Object()

//Above are two empty objects
```

---

# Object.assign
<p>
The Object.assign(target, ...sources) is a built-in JavaScript method that's used to copy the values of all enumerable properties from one or more source objects to a target object. It will return the modified target object.
</p>

```javascript
const obj1 = { a: 1 };
const obj2 = { b: 2 };
const obj3 = { c: 3 };

const merged = Object.assign({}, obj1, obj2, obj3);
console.log(merged); // Output: { a: 1, b: 2, c: 3 }
```
---
layout: center
---

# Welcome to DOM and EVENTS

---

# DOM

Known as the **Document Object Model**. It is the interface that allows interaction with and manipulation of HTML and CSS using JavaScript. The DOM is the webpage described as an object. With the DOM, you are able to:

- Access and modify HTML elements
- Change styles and attributes
- Handle events
- Create, delete, or move elements

---

## ACCESSING DOM ELEMENTS

### 🔹 By ID

The DOM can be accessed using element IDs.

```html
<div id="container">This is an example</div>

const container = document.getElementById("container");
```

### 🔹 By Class

The DOM can be accessed using class names.

```html
<span class="greet">Hey there!</span>

const greet = document.getElementsByClassName("greet");
```

---

### 🔹 By Tag name

The DOM can be accessed by using the Tag name

```html
<p>I am a paragraph</p>

const paragraphs = document.getElementsByTagName("p");
```

### 🔹 By Using querySelector/querySelectorAll

This is the most recommended way of accessing the DOM

```html
<h2 class="month">January</h2>
<h2 class="month">February</h2>
<h2 class="month">March</h2>
<h2 class="month">April</h2>
<h2 class="month">May</h2>

<script>
  const firstMonth = document.querySelector(".month");
  const allMonths = document.querySelectorAll(".month");
</script>
```

---

## CHANGING CONTENTS

### 🔹 Change Text

Replace the text inside an element.

```html
<h2 class="month">January</h2>

<script>
  const firstMonth = document.querySelector(".month");
  firstMonth.textContent = "New Month";
</script>
```

### 🔹 Change HTML

Replace the inner HTML structure of an element.

```html
<span class="greet">Hey there!</span>

<script>
  const greet = document.querySelector(".greet");
  greet.innerHTML = "<div>Inner HTML was changed</div>";
</script>
```

---

### 🔹 Creating and Inserting Elements

Create a new element and add it to the page

```html
<script>
  const newDiv = document.createElement("div"); // creates a div element
  newDiv.textContent = "I was created!"; // adds text content
  document.body.appendChild(newDiv); // appends to the body
</script>
```

### 🔹 Removing Elements

Use .remove() to delete an element from the DOM.

```html
<p>I am a paragraph</p>

<script>
  const paragraphs = document.getElementsByTagName("p");
  paragraphs[0].remove(); // removes the first paragraph
</script>
```

---

### 🔹 Changing styles

Use .style to modify CSS properties directly from JavaScript.

```html
<div class="design">My design</div>

<script>
  const design = document.querySelector(".design");
  design.style.color = "blue";
  design.style.fontSize = "24px";
</script>
```
---

# EVENTS
<div v-click>

Events are actions that occur in the browser (e.g., clicks, form submissions, key presses).  
JavaScript can respond to these actions using **event handlers**.

**Handlers** are functions that run in response to events.
</div>

<div v-click>

### 🔹 Common Event Types

- `click`: Triggered when an element is clicked  
- `submit`: Triggered when a form is submitted  
- `mouseover`: Triggered when the mouse hovers over an element  
- `keydown`: Triggered when a key is pressed  
- `input`: Triggered when the value of an input changes
- `change`: Triggered when the value of an input or select element is changed and loses focus

</div>
---

## WAYS OF HANDLING EVENTS

In JavaScript, there are three primary ways to handle events. Below are the three main methods for handling events:

<div v-click>

### 🔹 HTML Attribute Method  
In this method, the event handler is directly attached within the HTML element using an event attribute, such as `onclick`.

```html
<!--HTML-->
<button onclick="sayHello()">Click (HTML Attribute)</button>

<script>
  function sayHello() {
    alert("Hello from HTML attribute!");
  }
</script>
```
</div>
---

### 🔹 DOM Property Method
<div v-click>

This method uses JavaScript to assign the event handler to the corresponding event property of an element (e.g., onclick).

```html
<!--HTML-->
<button id="btn2">Click (DOM Property)</button>

<script>
  const btn2 = document.getElementById("btn2");
  btn2.onclick = function () {
    alert("Hello from DOM property!");
  };
</script>
```
</div>
---

### 🔹 addEventListener() Method
<div v-click>

This is the most flexible and recommended method for handling events. The addEventListener() method allows you to attach one or more event handlers to an element without overwriting existing ones.

```html
<!--HTML-->
<button class="btn3">Click (addEventListener)</button>

<script>
  const btn3 = document.querySelector(".btn3");

  function handleClick() {
    alert("I was clicked!!");
  }

  // You could also use an arrow function
  // const handleClick = () => alert("I was clicked!!");

  btn3.addEventListener("click", handleClick);
</script>
```
</div>
---
layout: center

---

# APPLICATION PROGRAMMING INTERFACE (API)
---

Application is any software that has a specific functionality. 
Interface is a protocol that dictates how two application talks to each other using requests and responses.
So put together, it is a way by which different systems or applications communicate with each other, thereby enabling them to share data and functionalities seamlessly. An API call is the act of making this request.

<h1>Why do we need APIs?</h1>
A non-technical analogy
<br>

Imagine making a reservation for four people at a restaurant. You will have to make a call to customer rep of the restaurant to make enquiries about availability, who in return would have to ask you to hold on for some seconds to confirm and get back to you with either a yes or no response.
The CS here is an API. It saves the client the stress of having to go through each departments to check for their availability. 
<br>

In technical terms, using the daily weather update on your mobile device is an example.
---

<h2>API calls typically include</h2>
<br>

- HTTP method: Specifies the type of request (e.g., GET, POST, PUT, DELETE)
- Headers: Provide additional information about the request (e.g., authentication tokens, content type)
- Payload: The data sent in the request (e.g., login credentials, booking details)
<br>

Making API calls in JavaScript is typically done using either the fetch() API or XMLHttpRequest, though fetch() is more modern and widely preferred.
```javascript
// Using fetch() to make a GET request
async function fetchWeatherData() {
  try {
    const res = await fetch("https://api.weather.com/current?city=Abuja"); // Making a GET request
    if (!res.ok) {
      throw new Error("Network response was not ok");
    }
    const data = await res.json();
    console.log(data); // Process the data
  } catch (error) {
    console.error("Error fetching weather data:", error);
  }
}
fetchWeatherData();
```
---
layout: center
---

# Promise and Async

<div v-click>fetch, async, await</div>

#### Promise

A Promise is a built-in JavaScript object that represents a value that may be available now, in the future, or never. It's used for handling asynchronous operations like loading data from a server.
---

Here is how to to write it:

<div v-click>

```js
let promise = new Promise((resolve, reject) => {
  // Simulate an asynchronous task, like a server request
  setTimeout(() => {
    let success = true; // Change to false to test reject
    if (success) {
      resolve("Task completed successfully!");
    } else {
      reject("Something went wrong.");
    }
  }, 1000);
});
// Using the promise
promise
  .then((result) => {
    console.log("Success:", result);
  })
  .catch((error) => {
    console.error("Error:", error);
  });
```

</div>

---

What’s happening:

- new Promise(...): Creates a new Promise object.
- resolve(...): Called when the task completes successfully.
- reject(...): Called when something goes wrong.
- .then(...): Runs if the promise is resolved.
- .catch(...): Runs if the promise is rejected.

---

### The fetch() API

<div v-click>

The `fetch()` API is a modern JavaScript method used to make HTTP requests, such as getting data from a server or an API. It is Promise-based, meaning it returns a Promise that resolves to a Response object.

</div>
<div v-click>

#### Key Features:

- Built into modern browsers (no need to install).
- Returns a Promise, which you can handle with `.then()` or `async/await.`
- Can make requests like `GET,` `POT,` `PUT,` `DELETE,` etc.
</div>

<div v-click>

#### How to write it with promise:

```js
fetch("https://official-joke-api.appspot.com/jokes/random")
  .then((response) => response.json()) // Convert response to JSON
  .then((data) => {
    console.log(`${data.setup} — ${data.punchline}`); // Display the joke
  })
  .catch((error) => {
    console.error("Error:", error); // Handle any errors
  });
```
</div>

---
layout: center
---

<h2>Async and await</h2>
---

<div v-click>

Before `async` and `await`, we used Promises and `.then()` to handle asynchronous code. But `async/await` is a cleaner, more readable way to handle the same thing.

</div>

<div v-click>

#### The `async` Function

</div>

<div v-click>

The `async` function is a function that always returns a Promise. Even if you don't explicitly return a Promise, JavaScript wraps the result inside a Promise.

</div>

<div v-click>

#### for example:

</div>

<div v-click>

```js
async function sayHi() {
  return "Hi!";
}
sayHi().then(console.log); // Output: "Hi!"
```

Even though we just returned a string, `sayHi()` becomes a Promise because of the `async` keyword.

</div>

---

<div v-click>

### The `await` block

</div>

await pauses until a Promise finishes

```js
async function getJoke() {
  let response = await fetch(
    "https://official-joke-api.appspot.com/jokes/random"
  );
  let data = await response.json();
  console.log(data.setup, data.punchline);
}
```
- await fetch(...) waits until the fetch finishes
- await response.json() waits until the JSON is ready
- Then we log the joke
Without await, the function would run ahead without waiting.
---

<div v-click>

### Handling Errors with `try...catch`

</div>
<div v-click>

try...catch works just like with normal code, and it catches Promise rejections or network errors.
```js
async function getJoke() {
  try {
    let res = await fetch("https://api.badurl.com");
    let data = await res.json();
    console.log(data);
  } catch (error) {
    console.error("Oops! Something went wrong:", error);
  }
}
```
</div>
---
layout: center
---

# Web Components

---

# Overview

- Basics

- Custom Elements

- Shadow DOM

---

# Basics

Web Components represent a significant leap forward in web development, offering
developers the ability to create reusable, encapsulated components that work
seamlessly across different frameworks and libraries. This introduction will
help you understand what Web Components are, why they matter, and how they can
transform your approach to building web applications.

# What are web components?

At their core, Web Components are a set of standardized web platform APIs that
allow you to create new, custom, reusable HTML elements. Imagine being able to
create your own custom-datepicker or advanced-carousel that works just like
native HTML elements such as select or video. That’s exactly what Web Components
enable!

# Why Web Components Matters

- Reusability: Can be reused or shared across different projects.
- Framework Independence: Works in any JavaScript framework.
- Encapsulation: Components are self-contained, hence improving security.

---

# What are The Three Pillars of Web Components?

1. Custom Elements
   - Define new HTML tags
   - Create custom elements behaviour
   - Extend existing HTML elements
2. Shadow DOM
   - Encapsulate styles and markup
   - Create a seperate DOM tree
   - Isolate components internals
3. HTML Templates
   - Define resuable markup
   - Create insert HTML fragments
   - Stamp out components instances
---
layout: center
---

# Modules and Dynamic Imports

---
layout: center
---

# Modules
- Module basics
- Export and Import
- Dynamic Imports
---

# What is a module?
A module is just a file. Modules can load each other and use special directives export and import to share functionality. Modularity is a key aspect of large-scale software development. It is the process of breaking a program into separate, interchangeable components that can be used in different parts of the program.

```html
<script src="" type="module"> </script>
```

Export keyword labels variables and functions that should be accessible from outside the current module then import allows the usage in other modules. Modules have come to JavaScript relatively recently. Before, there were no modules in JavaScript, and every script included in the HTML had access to all other scripts. Which could be a problem for global variables and functions and the order is important. So, modules are a way to solve these problems.

For instance, if we have a file menu.js exporting a function:
<div class="grid grid-cols-3 gap-5 pt-4 -mb-6">
```javascript
// 📁 menu.js
export function menu(user) {
  alert(`Hello, ${user}!`)
}
```
```javascript
// 📁 menu.js
export function menu(user) {
  alert(`Hello, ${user}!`)
}
export {menu}
```
```javascript
// 📁 script.js - named import
// because of a valid named export
import { menu } from './menu.js'
```
</div>
---

# What is Importing?
- Importing is the method by which you make exported code available in another JavaScript file. This is essential for assembling various components and libraries to build complex applications.
- Import * as "var name": This syntax allows you to import all exported code from a module and assign it to a single object. This is useful when you want to import multiple modules into a single file.
- Usually, we put a list of what to import in curly braces import.
- But if there’s a lot to import, we can import everything as an object using import * as "var name", for instance:
  
<div class="grid grid-cols-2 gap-5 pt-4 -mb-6">

```javascript
// 📁 script.js
import { name as name, age as age } from './bio.js'
function(name){
  console.log(`My name is ${name}, I am ${age} years old`);
}
```
```javascript
// 📁 script.js
import * as bio from './bio.js'

bio.name // SirJaey
bio.track // Frontend Engineering
```
</div>
---

# Dynamic Imports
- Dynamic imports revolutionize how modules are handled, offering a more flexible approach compared to static imports. Static imports require all modules to be loaded at the beginning of a script, increasing initial load times and potentially impacting performance. In contrast, dynamic imports load modules on demand, which can significantly reduce initial load times and enhance user experience.

<div class="grid grid-cols-2 gap-5 pt-4 -mb-6">

```javascript
// Static import (traditional method)
import { module } from './path/to/module.js'
```
```javascript
// Dynamic import
const module = await import('./path/to/module.js')
```
</div>
- 


- Explanation: The above example contrasts the traditional static import with a dynamic import. Notice that dynamic imports use a promise-based syntax, which means they can be used within asynchronous functions or handled with .then() and .catch() for greater control over timing and error handling.
- Dynamic imports are particularly beneficial in scenarios where parts of your application are conditionally used or not immediately necessary.
---
transition: fade
class: lead
layout: center
---

# Introduction to React.js
---
layout: center
class: heading
---
# Overview

- Introduction to React
- JSX (JavaScript XML)
- Components
- Example Codes

---

# What is React?

- **A JavaScript library** for building fast and interactive user interfaces.
- Created and maintained by **Facebook**.
- Focuses on building **reusable components**.

---
layout: center
---

# React Logo
![React Logo](https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg)

---

# What is JSX?

- JSX stands for **JavaScript XML**.
- It allows us to **write HTML** inside JavaScript.
- JSX makes writing React components **easier and more readable**.

---

# JSX Example

```jsx
const element = <h1>Hello, world!</h1>;

// Embedding JavaScript expressions
const name = "John";
const greeting = <h2>Hello, {name}!</h2>;
```


```jsx 
// Applying inline CSS styling in JSX
const headingStyle = {
  color: "blue",
  textAlign: "center"
};

const styledHeading = <h1 style={headingStyle}>Styled Heading</h1>

```

---

# JSX Example 2

-Use camelCase for CSS properties.

-Example: backgroundColor (✅) vs background-color (❌)

-The style attribute takes a JavaScript object.

-You can use external .css files too, but inline styles are handy for quick designs.

---

# React Components
Components are reusable building blocks in React.
They help organize the UI into small, manageable parts.
Props are passed to components like HTML attributes.
<br>

Components can be **functional** or **class-based**.
Components can accept **props** (properties) to make them dynamic.
- Functional Components (modern) are simpler and easier to read.
- Class Components (older) are more complex and used for state management.

---

# Components Functions
```jsx
// Basic Functional Component
function Welcome() {
  return <h1>Welcome to React!</h1>;
}
```
```jsx
// Component receiving props (dynamic data)
function GreetUser(props) {
  return <h2>Hello, {props.name}!</h2>;
}
```
```jsx
// Component with internal styling
function StyledMessage() {
  const messageStyle = { color: "green", fontSize: "20px" };
  return <p style={messageStyle}>This is a styled message!</p>;
}
```
---

# Combining Components

```jsx
function App() {
  return (
    <div>
      <Welcome />
      <GreetUser name="John" />
      <GreetUser name="Jane" />
      <StyledMessage />
    </div>
  );
}

```
---
layout: full
---

![Image](https://shorturl.at/jNJVV)

# Thank you for listening!
