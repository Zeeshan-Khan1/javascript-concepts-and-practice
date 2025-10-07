# JavaScript Functions

Functions are one of the most **important building blocks** in JavaScript.  
They allow developers to write **modular, reusable, and organized** code.

---

## What Are Functions?

A **function** is a block of code designed to perform a specific task.  
Functions execute when they are **called** (or **invoked**).

### Example: Multiply Two Numbers

```js
function myFunction(p1, p2) {
  return p1 * p2;
}
```
### JavaScript Function Syntax
```js
function name(p1, p2, p3) {
  // code to be executed
}
Syntax Breakdown:
function — Keyword to declare a function.

name — Function name (follows variable naming rules).

(p1, p2, p3) — Parameters (optional, comma-separated).

{ code } — Block of code to execute when the function is called.

A function can return a value back to the caller using the return keyword.
```
### Why Use Functions?
- Functions allow you to:
- Reuse code instead of rewriting it.
- Organize code into smaller, manageable sections.
- Use the same code with different arguments for different results.

### Function Invocation
The code inside a function executes when it is invoked.

Functions can be called:
From JavaScript code directly.
When an event occurs (like a button click).
Automatically (self-invoking functions).
The () operator is used to call a function.

### Example: Convert Fahrenheit to Celsius
```js
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}

let value = toCelsius(77);
Common Function Invocation Mistakes
Missing Arguments

function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}

let value = toCelsius();  // Incorrect usage

Missing Parentheses

function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}

let value = toCelsius;  // Returns the function itself, not the result
 toCelsius → refers to the function object
toCelsius() → refers to the function result
```
### Arrow Functions (ES6)
Arrow functions were introduced in ES6 to simplify syntax.

Before (Regular Function)
```js
let myFunction = function(a, b) {
  return a * b;
};
After (Arrow Function)

let myFunction = (a, b) => a * b;
Arrow functions are shorter and more concise, often used in modern JavaScript.
```
### Local Variables
Variables declared inside a function are local to that function and cannot be accessed outside of it.

Example:
```js
// code here cannot use carName

function myFunction() {
  let carName = "Volvo";
  // code here can use carName
}

// code here cannot use carName
Local variables are created when a function starts and deleted when it ends.
Variables with the same name can exist in different functions without conflict.
```
### Parameters vs. Arguments
Term	Description
Parameters	Names listed in the function definition.
Arguments	Actual values passed to the function when called.

Example (Parameters)
```js
function greet(name, age) {
  return `Hello ${name}! You are ${age} years old.`;
}
Example (Arguments)

greet("John", 21);
```
### Functions Used as Variables
Functions can be used as variable values in expressions, calculations, or string concatenation.

Example 1 – Using Variable
```js
let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
Example 2 – Using Function Directly

let text = "The temperature is " + toCelsius(77) + " Celsius";
```
