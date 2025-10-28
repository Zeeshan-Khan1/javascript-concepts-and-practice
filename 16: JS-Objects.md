# JavaScript Objects

In JavaScript, **objects** are variables that can hold multiple values as **key–value pairs**.  
They are one of the most powerful data types and form the backbone of JavaScript programming.

---
## What is an Object?

An **object** is a collection of related data and functionality — represented as **properties** and **methods**.

**Properties** are values associated with the object.  
**Methods** are actions (functions) that can be performed on the object.

---
### Example: Car Object

| **Car Properties** | **Car Methods** |
|---------------------|-----------------|
| `car.name = "Fiat"` | `car.start()` |
| `car.model = "500"` | `car.drive()` |
| `car.weight = "850kg"` | `car.brake()` |
| `car.color = "white"` | `car.stop()` |

Different cars share the same properties (like `model`, `color`),  
but their **values** and **method actions** can differ.

---

## Creating a JavaScript Object

You can assign multiple values to an object like this:

```js
const car = { type: "Fiat", model: "500", color: "white" };
//Always declare objects using const —
//It prevents reassignment but you can still modify its properties.
```
## Object Literals
An object literal is the simplest way to create an object:

```js
const person = { firstName: "John", lastName: "Doe", age: 50, eyeColor: "blue" };
Objects can also span multiple lines for better readability:

const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```
You can also create an empty object and add properties later:
```js
const person = {};
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue";
```
Using the new Object() Keyword
You can also create an object using the built-in constructor:
```js
const person = new Object({
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
});
```
Using new Object() is not recommended.
Always prefer object literals for simplicity, readability, and performance.

Accessing Object Properties
You can access object properties in two ways:
```
person.lastName;
person["lastName"];
```
JavaScript Object Methods
Object methods are functions stored as property values.
```js
Property	Value
firstName	"John"
lastName	"Doe"
age	50
eyeColor	"blue"
fullName	function() { return this.firstName + " " + this.lastName; }

//Example:

const person = {
  firstName: "John",
  lastName: "Doe",
  id: 5566,
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
};

//The keyword this refers to the current object.
//In this example, this.firstName means the firstName property of person.

## Displaying JavaScript Objects
Displaying an object directly outputs:

```js
[object Object]
//Example:
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

let text = person; // Outputs: [object Object]

## Displaying Object Properties
You can combine property values into a string:

```js
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

let text = person.name + ", " + person.age + ", " + person.city;
```
## Object Constructor Functions
Sometimes, you need to create many similar objects.
For this, we use a constructor function.

```js
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}
```

## Now you can create multiple instances:

```js
const myFather = new Person("John", "Doe", 50, "blue");
const myMother = new Person("Sally", "Rally", 48, "green");
const mySister = new Person("Anna", "Rally", 18, "green");
const mySelf = new Person("Johnny", "Rally", 22, "green");
```
## Summary
- Objects are containers for properties and methods.

- Properties are named values.

- Methods are functions stored as object properties.
- Constructor functions create multiple objects of the same type.

- Properties can hold values, functions, or even other objects.



