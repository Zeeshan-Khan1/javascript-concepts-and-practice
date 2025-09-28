# JavaScript Strings

### Strings in JavaScript are used for storing and manipulating text. They are written inside quotes.

### Using Quotes

A string can be defined with single or double quotes:
```
let carName1 = "Volvo XC60";  // Double quotes
let carName2 = 'Volvo XC60';  // Single quotes
```

### ✅ Both work the same.

Quotes Inside Quotes

You can use quotes inside a string, as long as they don’t match the surrounding ones:
```
let answer1 = "It's alright";
let answer2 = "He is called 'Johnny'";
let answer3 = 'He is called "Johnny"';
```
### Template Strings (ES6+)

Template literals use backticks (` `). They allow:

Single and double quotes inside

Multiline strings

Variable embedding with ${}
```
let name = "Johnny";
let text = `He's often called "Johnny"`;
let multiLine = `The quick
brown fox
jumps over
the lazy dog`;
```
### String Length

Use .length to find the number of characters:
```
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = text.length;  // 26
```
### Escape Characters

If you need special characters inside strings, use a backslash (\) escape:
```
Code	Result	Description
\'	'	Single quote
\"	"	Double quote
\\	\	Backslash
\n	New line	Line break
\t	Tab	Horizontal tab

Examples:

let text1 = "We are the so-called \"Vikings\" from the north.";
let text2 = 'It\'s alright.';
let text3 = "The character \\ is called backslash.";
```
Breaking Long Lines

To improve readability:
```
document.getElementById("demo").innerHTML =
"Hello Dolly!";

document.getElementById("demo").innerHTML =
"Hello " + "Dolly!";

Strings as Objects (⚠️ Not Recommended)

Normally, strings are primitive values:

let x = "John";


But they can also be created as objects:

let y = new String("John");


⚠️ Avoid this! It complicates code and may give unexpected results:

let x = "John";
let y = new String("John");

console.log(x == y);  // true
console.log(x === y); // false
```

Comparing two string objects always returns false.

### ✅ Quick Recap

Use quotes (' or ") for normal strings.

Use backticks (` `) for templates, multiline, and embedded variables.

Use .length to count characters.

Use escape characters for quotes, backslashes, and line breaks.

❌ Avoid creating strings with new String().

👉 Next: JavaScript String Methods
