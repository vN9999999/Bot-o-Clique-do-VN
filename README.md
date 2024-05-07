# Bot-o-Clique-do-VN
Botão top
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Botão Piscante</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            background-color: black;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            color: white;
            font-family: Arial, sans-serif;
        }
        #botaoClique {
            font-size: 24px;
            background-color: red;
            color: white;
            border: none;
            padding: 20px;
            border-radius: 10px;
            cursor: pointer;
            animation: blink 1s infinite;
        }
        @keyframes blink {
            0% { opacity: 0; }
            50% { opacity: 1; }
            100% { opacity: 0; }
        }
        #mensagem {
            display: none;
            margin-top: 20px;
        }
        #carinhaFeliz {
            font-size: 48px;
            color: blue;
            display: none;
        }
    </style>
</head>
<body>
    <button id="botaoClique" onclick="mostrarMensagem()">Clique</button>
    <div id="mensagem"></div>
    <div id="carinhaFeliz">😊</div>

    <script>
        function mostrarMensagem() {
            document.getElementById('botaoClique').style.display = 'none';
            document.getElementById('mensagem').innerText = 'Clicou';
            document.getElementById('mensagem').style.display = 'block';
            document.getElementById('carinhaFeliz').style.display = 'block';
            // Adicione aqui o código para tocar a música alegre
        }
    </script>
</body>
</html>
