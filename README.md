<!DOCTYPE html>
<html>
<!-- Augmented Reality Sample demonstration by Zesty, 12.28.22 -->
<head>
    <title>Augmented Reality</title>
    <script>
        // Defining the function
        function changePersp(value) {
            document.getElementById('div1').style.perspective = value + "px";
            document.getElementById('persp').innerHTML = value;
        }
    </script>
</head>
<body onload="changePersp(200);">
    <div id="h1"><h1>Augmented Reality Sample</h1></div>

    <div id="div1">
        <div id="div2">HELLO Welcome to HCI</div>
    </div>
    
    <br>
    Change Perspective:<br>
    <input type="range" min="45" max="2000" value="200" onchange="changePersp(this.value)" /><br>
</body>
<style>
    #div1 {
        position: relative;
        height: 200px;
        width: 200px;
        margin: 50px;
        padding: 10px;
        border: 1px solid red;
        align-content: center;
    }

    #div2 {
        padding: 50px;
        position: absolute;
        border: 1px solid red;
        background-color: green;
        transform: rotateX(45deg);
        text-align: center;
        align-content: center;
    }

    #h1 {
        background-color: lemonchiffon;
        text-align: center;
        font-style: oblique;
    }
</style>
</html>


