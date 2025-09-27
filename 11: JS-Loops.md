# JavaScript Loops

Loops allow you to execute a block of code multiple times.  
They are especially useful when working with arrays or repetitive tasks.

---

## Why Loops?

Instead of writing code repeatedly:

```js
text += cars[0] + "<br>";
text += cars[1] + "<br>";
text += cars[2] + "<br>";
```

You can use a loop:
```js
for (let i = 0; i < cars.length; i++) {
  text += cars[i] + "<br>";
}
```
### 1. The for Loop
The for statement creates a loop with 3 expressions:
```js
for (expr1; expr2; expr3) {
  // code block
}
expr1 → runs once before the loop starts

expr2 → condition checked before each iteration

expr3 → executed after every iteration
```
### Example
```
for (let i = 0; i < 5; i++) {
  console.log("The number is " + i);
}
expr1: initializes (let i = 0)

expr2: condition (i < 5)

expr3: increment (i++)
```
### Loop Scope
```js
let i = 5;

for (i = 0; i < 10; i++) {
  // some code
}
// Here i is 10

let i = 5;

for (let i = 0; i < 10; i++) {
  // some code
}
// Here i is still 5
Declaring with let inside the loop makes i scoped to that loop.
```
### 2. The while Loop
Runs as long as the condition is true.

### Syntax
```js
while (condition) {
  // code block
}
Example

let i = 0;
while (i < 10) {
  console.log("The number is " + i);
  i++;
}
```
⚠️ If you forget to update the variable, the loop can run forever.

### 3. The do...while Loop
Executes at least once, even if the condition is false.

### Syntax
```js
do {
  // code block
} while (condition);
Example

let i = 0;
do {
  console.log("The number is " + i);
  i++;
} while (i < 10);
:
```
### ✅ Use
- for → when you know the number of iterations.

- while → when you don’t know how many times to run.

- do...while → when you want the loop to run at least once.
