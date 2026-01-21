<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Proyecto</title>
    <style>
        body {
            background-color: #121212;
            color: #ffffff;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
        }
        h1 {
            color: #ffffff;
            font-size: 4rem;
            margin: 0;
        }
        p {
            color: #cccccc;
            font-size: 2rem;
            margin: 20px 0 0 0;
        }
        button {
            background-color: #333333;
            color: #ffffff;
            border: none;
            padding: 15px 30px;
            margin: 20px 10px;
            font-size: 1.5rem;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #555555;
        }
        .buttons {
            display: flex;
            justify-content: center;
            margin-top: 40px;
        }
        @keyframes shake {
            0% { transform: translateX(0); }
            25% { transform: translateX(-10px); }
            50% { transform: translateX(10px); }
            75% { transform: translateX(-10px); }
            100% { transform: translateX(0); }
        }
        .shake {
            animation: shake 0.5s;
        }
    </style>
</head>
<body> 
    <h1>ENTONCES HACEMOS LA PAGINA O MIEDO? </h1>
    <p></p>
    <div class="buttons">
        <button>Sí</button>
        <button>No</button>
    </div>
    <div id="message" style="display:none; margin-top:40px; text-align:center; font-size:1.5rem; color:#cccccc;">
        <p>hola mano, si esta mirando esto es porque puso que si ahora toca crear la pagina y empezar a hacerle, escribame aqui</p>
        <img src="whapyojan.jpeg" alt="whapyojan" style="max-width:80%; margin-top:20px; border-radius:10px;">
    </div>
    <div id="noMessage" style="display:none; margin-top:40px; text-align:center; font-size:1.5rem; color:#ff0000;">
        <p>mono marica</p>
        <img src="gatodedo.jpg" alt="gatodedo" style="max-width:80%; margin-top:20px; border-radius:10px;">
    </div>
    <script>
        document.querySelector('.buttons button:first-child').addEventListener('click', () => {
            document.getElementById('message').style.display = 'block';
        });
        document.querySelector('.buttons button:last-child').addEventListener('click', () => {
            document.getElementById('noMessage').style.display = 'block';
        });
    </script>
</body>
</html>
