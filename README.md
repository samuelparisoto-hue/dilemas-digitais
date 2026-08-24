# dilemas-digitais
HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delitos Digitais</title>
    <style>
        body {
            background-color: #121212;
            color: #ffffff;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
        }

        header {
            background-color: #1e1e1e;
            text-align: center;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        header h1 {
            color: #ff4d4d;
            margin: 0;
        }

        main {
            max-width: 600px;
            margin: 0 auto;
        }

        article {
            background-color: #1e1e1e;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 5px solid #ff4d4d;
        }

        h2 {
            margin-top: 0;
            color: #ff4d4d;
        }

        .autor {
            color: #888888;
            font-weight: bold;
        }

        button {
            background-color: #333333;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #555555;
        }

        footer {
            text-align: center;
            color: #888888;
            margin-top: 30px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Blog sobre Delitos Digitais</h1>
        <p>Aprenda a se proteger de golpes na internet</p>
    </header>

    <main>
        <article>
            <h2>Cuidado com o Golpe do Phishing</h2>
            <p class="autor">Por: Alexandra</p>
            <p>O phishing é quando golpistas enviam links falsos por mensagem ou e-mail fingindo ser bancos ou lojas para roubar suas senhas.</p>
            <button>❤️ <span>0</span></button>
        </article>

        <article>
            <h2>Como Proteger Suas Senhas</h2>
            <p class="autor">Por: Alexandra</p>
            <p>Não use a mesma senha para tudo! Crie senhas fortes misturando letras, números e símbolos para evitar que invadam suas contas.</p>
            <button>❤️ <span>0</span></button>
        </article>
    </main>

    <footer>
        <p>Desenvolvido por Alexandra</p>
    </footer>

    <script>
        const botoes = document.querySelectorAll("button");

        botoes.forEach(function(botao) {
            let curtiu = false;

            botao.addEventListener("click", function() {
                let contador = botao.querySelector("span");
                
                if (!curtiu) {
                    contador.textContent = Number(contador.textContent) + 1;
                    curtiu = true;
                } else {
                    contador.textContent = Number(contador.textContent) - 1;
                    curtiu = false;
                }
            });
        });
    </script>

</body>
</html>d

