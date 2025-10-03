# JavaScript Numbers

- JavaScript has only one type of number.
- Numbers can be written with or without decimals.
```js
let x = 3.14;   // Number with decimals
let y = 3;      // Number without decimals
```

### Extra large or small numbers use scientific notation:
```js
let x = 123e5;   // 12300000
let y = 123e-5;  // 0.00123
```
### Numbers in JavaScript

- JavaScript numbers are always 64-bit floating point (IEEE 754 standard).

- No separate types like int, float, double → all are just Number.

### Breakdown of 64 bits:

- 52 bits → fraction (value)

- 11 bits → exponent

- 1 bit → sign

Integer Precision

Integers are accurate up to 15 digits:
```js
let x = 999999999999999;   // 15 digits → OK
let y = 9999999999999999;  // 16 digits → Rounded
```

Decimal precision is up to 17 digits.

Floating Precision

Floating point arithmetic is not always exact:

let x = 0.2 + 0.1;   // 0.30000000000000004


### Fix: Multiply and divide:
```js
let x = (0.2 * 10 + 0.1 * 10) / 10;  // 0.3
```
### Adding Numbers and Strings

The + operator is used for both addition and concatenation.
```js
let x = 10;
let y = 20;
let z = x + y;   // 30 → number

let x = "10";
let y = "20";
let z = x + y;   // "1020" → string
```

### Mixing strings and numbers:
```js
let x = 10;
let y = "20";
let z = x + y;   // "1020"
```

### Be careful!
```js
let x = 10;
let y = 20;
let z = "The result is: " + x + y;  // "The result is: 1020"
```
### Numeric Strings

JavaScript tries to convert strings to numbers in math operations (except +):
```js
"100" / "10"   // 10
"100" * "10"   // 1000
"100" - "10"   // 90
"100" + "10"   // "10010" (concatenation)

NaN (Not a Number)

NaN means “Not a Number”.

let x = 100 / "Apple";  // NaN
let y = 100 / "10";     // 10


Check with isNaN():

let x = 100 / "Apple";
console.log(isNaN(x));  // true
```

### Any operation with NaN → result is also NaN.
```js
let x = NaN;
let y = 5;
console.log(x + y);   // NaN

Infinity

Returned when a number exceeds the largest possible value:

let myNumber = 2;
while (myNumber != Infinity) {
  myNumber *= myNumber;
}


Division by zero also gives Infinity:

2 / 0;   // Infinity
-2 / 0;  // -Infinity
```

### typeof Infinity → "number"
```js
Hexadecimal & Number Bases

0x prefix = Hexadecimal

let x = 0xFF;   // 255
```

### Convert numbers to other bases with .toString(base):
```js
let n = 32;
n.toString(16);  // "20" (hex)
n.toString(2);   // "100000" (binary)

Numbers as Objects ( Not Recommended)

Numbers are normally primitive values:

let x = 123;


But can also be created as objects:

let y = new Number(123);
```

### Avoid this → slower and can cause issues:
```js
let x = 500;
let y = new Number(500);

console.log(x == y);   // true
console.log(x === y);  // false


Comparing two number objects:

let a = new Number(500);
let b = new Number(500);

console.log(a == b);   // false
console.log(a === b);  // false
```
### Quick Recap

All numbers in JS are 64-bit floating point.

Integers precise up to 15 digits.

Floating point may have rounding errors.

+ → addition for numbers, concatenation for strings.

NaN and Infinity are numbers too (typeof returns "number").

Avoid new Number() — always use number literals.

Next: JavaScript Number Methods
