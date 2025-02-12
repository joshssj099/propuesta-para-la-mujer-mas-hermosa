# propuesta-para-la-mujer-mas-hermosa
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            position: relative;
        }

        .container {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            position: relative;
            z-index: 2;
        }

        h1 {
            color: #ff4d4d;
        }

        .buttons {
            margin-top: 20px;
        }

        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            transition: 0.3s;
        }

        #yes {
            background-color: #ff4d4d;
            color: white;
        }

        #yes:hover {
            background-color: #e60000;
        }

        #no {
            background-color: #ccc;
            color: black;
            position: absolute;
        }

        /* Stickers flotantes */
        .sticker {
            position: absolute;
            width: 60px;
            height: 60px;
            animation: float 5s infinite ease-in-out;
        }

        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0); }
        }

        /* Imagen de confirmación */
        #love-img {
            display: none;
            margin-top: 20px;
            width: 150px;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Quieres ser mi San Valentín? ❤️</h1>
        <div class="buttons">
            <button id="yes" onclick="aceptar()">Sí</button>
            <button id="no" onmouseover="moverNo()">No</button>
        </div>
        <img id="love-img" src="https://i.pinimg.com/originals/5c/b5/9e/5cb59eecb69f4e9ac69f9df46c53b80c.png" alt="Pareja enamorada">
    </div>

    <!-- Stickers flotantes -->
    <img class="sticker" src="https://i.pinimg.com/originals/9d/d8/5d/9dd85d0d08e2a6d5e8f5f9a66fa391c5.png" style="top: 10%; left: 20%;">
    <img class="sticker" src="https://i.pinimg.com/originals/34/45/6b/34456b530db176c69c8dba0643cbe9c9.png" style="top: 30%; left: 70%;">
    <img class="sticker" src="https://i.pinimg.com/originals/8e/1a/5e/8e1a5ea9cf6d5a84b6fdb3792a3f1165.png" style="top: 60%; left: 10%;">
    <img class="sticker" src="https://i.pinimg.com/originals/b3/91/91/b39191bc97ff5e3e7ed645eafbb6a1e4.png" style="top: 80%; left: 50%;">

    <script>
        function aceptar() {
            alert("¡Sabía que dirías que sí! ❤️🥰");
            document.getElementById("love-img").style.display = "block";
        }

        function moverNo() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 100);
            document.getElementById("no").style.left = `${x}px`;
            document.getElementById("no").style.top = `${y}px`;
        }
    </script>

</body>
</html>
