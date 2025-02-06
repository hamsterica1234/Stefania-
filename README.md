<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vrei să fii Valentina mea?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
            background-color: #ffe6e6;
        }
        h1 {
            color: #d63384;
        }
        .container {
            margin-top: 30px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .btn-da {
            background-color: #ff4d4d;
            color: white;
        }
        .btn-nu {
            background-color: #666;
            color: white;
        }
        .hidden {
            display: none;
        }
        .inimioara {
            font-size: 50px;
            color: red;
        }
    </style>
</head>
<body>

    <h1>Vrei să fii Valentina mea?</h1>
    
    <div class="container">
        <button class="btn-da" onclick="showLove()">Da</button>
        <button class="btn-nu" onclick="moveNo()">Nu</button>
    </div>

    <div id="loveMessage" class="hidden">
        <p class="inimioara">❤️</p>
        <h2>Te iubesc, Ștefania!</h2>
    </div>

    <script>
        function showLove() {
            document.getElementById("loveMessage").classList.remove("hidden");
        }

        function moveNo() {
            let btnNu = document.querySelector('.btn-nu');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 100);
            btnNu.style.position = "absolute";
            btnNu.style.left = x + "px";
            btnNu.style.top = y + "px";
        }
    </script>

</body>
</html>
