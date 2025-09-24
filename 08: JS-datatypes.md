# JavaScript Datatypes

JavaScript variables can hold **8 different datatypes**.

---

## 📌 List of Datatypes
| Type       | Description                                    |
|------------|--------------------------------|
| **String**   | A sequence of characters inside quotes |
| **Number**   | Numeric value (integer or decimal) |
| **BigInt**   | Large integer values beyond `Number` range |
| **Boolean**  | `true` or `false` |
| **Object**   | Collection of key–value pairs |
| **Undefined** | Declared but not assigned a value |
| **Null**     | Intentional absence of value |
| **Symbol**   | Unique identifier (primitive) |

---

## 📌 Examples

### String
```javascript
let color = "Yellow";
let lastName = "Johnson";

Number
let length = 16;
let weight = 7.5;

BigInt
let x = 1234567890123456789012345n;
let y = BigInt(1234567890123456789012345);

Boolean
let isTrue = true;
let isFalse = false;

Object
const person = { firstName: "John", lastName: "Doe" };

Array (Object)
const cars = ["Saab", "Volvo", "BMW"];

Date (Object)
const date = new Date("2022-03-25");

Undefined
let x;

Null
let x = null;

Symbol
const id1 = Symbol();
const id2 = Symbol();

📌 The typeof Operator

Use typeof to check the datatype of a variable:

typeof ""        // "string"
typeof "John"    // "string"
typeof 0         // "number"
typeof 3.14      // "number"
typeof (3 + 4)   // "number"

📌 Strings in JavaScript

Strings are written inside quotes (single or double).

let car1 = "Volvo XC60"; // Double quotes
let car2 = 'Volvo XC60'; // Single quotes


Quotes inside strings:

let answer1 = "It's alright";
let answer2 = "He is called 'Johnny'";
let answer3 = 'He is called "Johnny"';

📌 Numbers in JavaScript

All numbers are floating point (decimal) by default.

let x1 = 34.00;  // With decimals
let x2 = 34;     // Without decimals


Exponential notation:

let y = 123e5;   // 12300000
let z = 123e-5;  // 0.00123

📌 Booleans

Booleans represent truth values: true or false.

let x = 5;
let y = 8;

console.log(x == 8); // false
console.log(x != 8); // true
console.log(x > 8);  // false
console.log(x < 8);  // true

📌 Undefined

A variable without a value has the type undefined.

let carName;
console.log(typeof carName); // "undefined"

📌 Empty Values

An empty value ("") is not the same as undefined.

let car = "";  // Value = "", typeof = "string"
