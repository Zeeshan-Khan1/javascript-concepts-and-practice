# JavaScript Introduction

## What is JavaScript?
JavaScript is the **programming language of the web**. It enables interactive web pages and is an essential part of modern web applications.  

- **HTML** defines the content  
- **CSS** specifies the layout and presentation  
- **JavaScript** programs the behavior and interactivity  

In short, JavaScript makes web pages **dynamic** and **interactive**.

---

## Key Capabilities of JavaScript
- Update and change both **HTML** and **CSS**  
- Calculate, manipulate, and validate data  
- Respond to **user interactions**  
- Create **animations and visual effects**  
- Handle **asynchronous operations**  

---

## Why Study JavaScript?
JavaScript is one of the **three core technologies of the World Wide Web** that every web developer must learn:

1. **HTML** → Defines the content structure of web pages  
2. **CSS** → Specifies the layout and design of web pages  
3. **JavaScript** → Programs the behavior and interactivity of web pages  

JavaScript runs on **virtually every device with a web browser**, making it one of the most widely used programming languages in history.

---

## JavaScript Can Change HTML Content
One of many JavaScript HTML methods is **`getElementById()`**.  
This method allows JavaScript to **locate and manipulate specific elements** in an HTML document.

**Example:**  
```html
<p id="demo">Original text</p>

<script>
  document.getElementById("demo").innerHTML = "Hello JavaScript";
</script>
