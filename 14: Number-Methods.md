# JavaScript Number Methods

JavaScript provides several **built-in methods** to work with numbers. These methods allow conversion, formatting, and validation of numeric data.

---

## 📘 Basic Methods

Basic number methods can be used on **any number**:

- `toString()`
- `toExponential()`
- `toFixed()`
- `toPrecision()`
- `valueOf()`

---

## ⚙️ Static Methods

Static methods belong to the **Number object** and can only be used like `Number.methodName()`:

- `Number.isFinite()`
- `Number.isInteger()`
- `Number.isNaN()`
- `Number.isSafeInteger()`
- `Number.parseInt()`
- `Number.parseFloat()`

---

## 🔢 The `toString()` Method

Converts a number into a string.

```js
let x = 123;
x.toString();
(123).toString();
(100 + 23).toString();
You can also specify a base (radix):

js
Copy code
let x = 123;
x.toString(2);  // Convert to binary
💥 The toExponential() Method
Returns a string with the number written in exponential notation.

js
Copy code
let x = 9.656;
x.toExponential(2);
x.toExponential(4);
x.toExponential(6);
💰 The toFixed() Method
Returns a string, rounding the number to a fixed number of decimal places.

js
Copy code
let x = 9.656;
x.toFixed(0);
x.toFixed(2);
x.toFixed(4);
x.toFixed(6);
💡 Useful for financial calculations.

✨ The toPrecision() Method
Returns a string with a number written with a specified length.

js
Copy code
let x = 9.656;
x.toPrecision();
x.toPrecision(2);
x.toPrecision(4);
x.toPrecision(6);
🧮 The valueOf() Method
Returns the primitive value of a number.

js
Copy code
let x = 123;
x.valueOf();
(123).valueOf();
(100 + 23).valueOf();
🔄 Converting Variables to Numbers
You can convert variables into numbers using:

Method	Description
Number()	Converts argument to a number
parseFloat()	Converts string to a floating number
parseInt()	Converts string to an integer

Example
js
Copy code
Number(true);
Number(false);
Number("10.33");
parseInt("10 years");
parseFloat("10.33");
If conversion fails, JavaScript returns NaN (Not a Number).

🕓 Number from Dates
You can also convert a Date into a number (milliseconds since 1970):

js
Copy code
Number(new Date("1970-01-01")); // 0
Number(new Date("1970-01-02")); // 86400000
Number(new Date("2017-09-30"));
🧩 The parseInt() Method
Parses a string and returns a whole number.

js
Copy code
parseInt("-10");
parseInt("-10.33");
parseInt("10 20 30");
parseInt("10 years");
parseInt("years 10"); // NaN
🧠 The parseFloat() Method
Parses a string and returns a floating-point number.

js
Copy code
parseFloat("10");
parseFloat("10.33");
parseFloat("10 20 30");
parseFloat("10 years");
parseFloat("years 10"); // NaN
🧱 Number Object Methods
Method	Description
Number.isInteger()	Checks if the value is an integer
Number.isNaN()	Checks if the value is NaN
Number.isFinite()	Checks if the value is finite
Number.isSafeInteger()	Checks if the value is a safe integer
Number.parseFloat()	Converts string to number
Number.parseInt()	Converts string to whole number

❌ Note: You cannot use x.isInteger() — it will throw an error.

✅ Examples
Number.isInteger()
js
Copy code
Number.isInteger(10);   // true
Number.isInteger(10.5); // false
Number.isFinite()
js
Copy code
Number.isFinite(123);     // true
Number.isFinite(Infinity); // false
Number.isNaN()
js
Copy code
Number.isNaN(123);   // false
Number.isNaN("abc"); // false
Number.isNaN(NaN);   // true
Number.isSafeInteger()
A safe integer can be accurately represented in JavaScript.

js
Copy code
Number.isSafeInteger(10);                  // true
Number.isSafeInteger(12345678901234567890); // false
Safe range: -(2⁵³ - 1) to +(2⁵³ - 1)
✅ Safe: 9007199254740991
❌ Unsafe: 9007199254740992

🧮 Number.parseFloat() & Number.parseInt()
Work the same as their global counterparts:

js
Copy code
Number.parseFloat("10.33");
Number.parseInt("10 20 30");
