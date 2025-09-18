# JavaScript Placement Options

## 1. In the `<head>` Section
```html
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
