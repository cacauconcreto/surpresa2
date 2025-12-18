<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quer sair comigo?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f8ff;
        }

        h1 {
            color: #333;
        }

        .botoes {
            position: relative;
            width: 300px;
            height: 100px;
            display: flex;
            justify-content: space-around;
            align-items: center;
        }

        button {
            padding: 15px 30px;
            font-size: 18px;
            cursor: pointer;
            border: none;
            border-radius: 10px;
            transition: transform 0.2s;
        }

        #btn-sim {
            background-color: #28a745;
            color: white;
        }

        #btn-nao {
            background-color: #dc3545;
            color: white;
            position: absolute; /* Necessário para mover livremente */
        }
    </style>
</head>
<body>

    <h1 id="pergunta">Você aceita tomar um café comigo? ☕</h1>

    <div class="botoes">
        <button id="btn-sim" onclick="aceitou()">Sim</button>
        <button id="btn-nao" onmouseover="fugir()" onclick="fugir()">Não</button>
    </div>

    <script>
        function fugir() {
            const btnNao = document.getElementById('btn-nao');
            
            // Calcula posições aleatórias dentro da janela
            // Subtraímos uma margem para o botão não sair da tela
            const larguraJanela = window.innerWidth - 100;
            const alturaJanela = window.innerHeight - 50;

            const novaPosicaoX = Math.random() * larguraJanela;
            const novaPosicaoY = Math.random() * alturaJanela;

            // Aplica as novas posições
            btnNao.style.position = 'fixed';
            btnNao.style.left = novaPosicaoX + 'px';
            btnNao.style.top = novaPosicaoY + 'px';
        }

        function aceitou() {
            const h1 = document.getElementById('pergunta');
            h1.innerHTML = "Agora sim! Sabia que ia aceitar! ❤️";
            
            // Esconde o botão não após o sim
            document.getElementById('btn-nao').style.display = 'none';
            // Aumenta o botão sim
            document.getElementById('btn-sim').style.transform = 'scale(1.5)';
        }
    </script>

</body>
</html>
