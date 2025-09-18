1. In the <head> Section
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
2. In the <body> Section (Recommended)
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
3. External JavaScript Files
External file: script.js

javascript
function changeText() {
    document.getElementById("demo").innerHTML = "Text changed!";
}
HTML file:

html
<!DOCTYPE html>
<html>
<body>
    <p id="demo">Original text</p>
    <button onclick="changeText()">Click me</button>
    
    <script src="script.js"></script>
</body>
</html>
