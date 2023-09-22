# Site-Curso-Bradesco

### JAVASCRIPT

```js
'use strict'
const switcher = document.querySelector('.btn');
switcher.addEventListener('click',function(){
    document.body.classList.toggle("dark-theme")

    var className = document.body.className;
    if(className == "light-theme"){
        this.textContent = "Dark";
    }
    else{
        this.textContent = "Light";
    }
    console.log('current class name: ' + className);
});
```

### INDEX
```html
<!DOCTYPE html>
<html lang="pt-be">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SITE CURSO</title>
    <link rel="stylesheet" href="main.css">
</head>
<body class="dark-theme">
    <h1>Task List</h1>
    <p id="msg">Current Tasks:</p>
    <ul>
        <li class="list">Add visual styles</li>
        <li class="list">Add light and dark themes</li>
        <li>Enable switching thee theme</li>
    </ul>
    <div>
        <button class="btn">Dark</button>
    </div>
    <script src="app.js"></script>
    <noscript>You need to enable JavaScipt to view the full site</noscript>
</body>
</html>
```

### CSS

```css
*{
    color: var(--fontColor);
    font-family: helvetica;
}
body{
    background: var(--bg);
}
ul{
    font-family: helvetica;
}
li{
    list-style: circle;
}
.list{
    list-style: square;
}
.light-theme{
    --bg: var(--green);
    --fontColor: var(--black);
    --btnBg: var(--black);
    --btnFontColor: var(--white);
}
.dark-theme{
    --bg: var(--black);
    --fontColor: var(--green);
    --btnBg: var(--white);
    --btnFontColor: var(--black);
}
.btn{
    position: absolute;
    top: 20px;
    left: 250px;
    height: 50px;
    width: 50px;
    border-radius: 50%;
    border: none;
    color: var(--btnFontColor);
    background-color: var(--btnBg);
}
.btn:focus{
    outline-style: none;
}
:root{
    --green: #00FF00;
    --white: #ffffff;
    --black: #000000;
}
```
