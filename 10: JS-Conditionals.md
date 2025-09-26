# JavaScript Conditionals

Conditional statements allow you to run different code depending on whether a condition is **true** or **false**.

---

## Types of Conditionals

- `if`
- `if...else`
- `if...else if...else`
- `switch`
- Ternary `? :`

---

## When to Use

- **if** → run code if a condition is true.  
- **else** → run code if the same condition is false.  
- **else if** → test a new condition if the first one is false.  
- **switch** → run one of many possible code blocks.  
- **ternary (? :)** → shorthand for `if...else`.  

---

## The `if` Statement

### Syntax
```js
if (condition) {
  // code to execute if the condition is true
}
The else Statement
Syntax
js

if (condition) {
  // code if true
} else {
  // code if false
}
The else if Statement
Syntax
js

if (condition1) {
  // code if condition1 is true
} else if (condition2) {
  // code if condition1 is false and condition2 is true
} else {
  // code if all conditions are false
}
The switch Statement
Use switch to test one value against multiple cases.

Syntax
js

switch (expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
Ternary Operator ? :
A shorthand for if...else.

Example
js

let age = 18;
let result = (age >= 18) ? "Adult" : "Minor";
console.log(result); // "Adult"
