<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            display: flex;
            justify-content: center;
            font-size: large;
        }
        .num{
            display: flex;
            text-align: center;
            margin-left: 15px;
        }
    </style>
</head>
<body>
    <center>
       <div class="num">
        <div id="a">0</div>+
        <div id="b">0</div> =
        <div id="eq">0</div>
    </div> 

        <button id="aB" onclick="aFunction()">A</button>
        <button id="bB" onclick="bFunction()">B</button>
        <button id="clear" onclick="clear()">clear</button>
    </center>
    <script>
        var clear = document.getElementById("clear")
        var a = document.getElementById("a");
        var b = document.getElementById("b");
        var eq = document.getElementById("eq")
        var aValue = 0;
        var bValue = 0;

        function aFunction(){
            aValue = Number(prompt("enter number", aValue))
            a.innerHTML = aValue;
            eq.innerHTML = aValue+bValue
        }

        function bFunction(){
            bValue = Number(prompt("enter number B",bValue ))
            b.innerHTML = bValue;
            eq.innerHTML = bValue+aValue
        }
        function clear(){
            aValue = 0;
            bValue = 0;
            a.innerHTML = "0";
            b.innerHTML = "0";
        }
    </script>
</body>
</html>
