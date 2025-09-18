# 2. In the <body> Section (Recommended)
```html
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
