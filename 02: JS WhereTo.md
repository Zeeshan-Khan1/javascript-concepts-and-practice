# JavaScript – Where To

## The `<script>` Tag
In HTML, JavaScript code is written between `<script>` and `</script>` tags.

**Example:**
```html
<script>
  document.getElementById("demo").innerHTML = "My First JavaScript";
</script>

# Placement Options
## 1. In the <head> Section
html
<!DOCTYPE html>
<html>
<head>
    <script>
    function changeText() {
        document.getElementById("demo").innerHTML = "Text changed!";
    }
    </script>
</head>
<body>
    <p id="demo">Original text</p>
    <button onclick="changeText()">Click me</button>
</body>
</html>
# 2. In the <body> Section (Recommended)
html
<!DOCTYPE html>
<html>
<body>
    <p id="demo">Original text</p>
    <button onclick="changeText()">Click me</button>
    
    <script>
    function changeText() {
        document.getElementById("demo").innerHTML = "Text changed!";
    }
    </script>
</body>
</html>
## Performance Tip: Place scripts at the bottom of the <body> for faster page loading.

# External JavaScript Files
## Create separate .js files for better organization:

script.js:

javascript
function changeText() {
    document.getElementById("demo").innerHTML = "Text changed!";
}
