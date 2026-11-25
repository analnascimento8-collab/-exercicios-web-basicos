# -exercicios-web-basicos
-  ATIVIDADE SENAI - 25 DE NOVEMBRO 2026  -
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------             
ATIVIDADE QUESTÂO 01 # (HTML5 - Estrutura Semântica e Formulário Simples)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
HTML

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title> Estrutura Semântica e Formulário Simples</title>
</head>
<body>

    <header>
        <h1> Página 25 de novembro 2026 </h1>
    </header>

    <main>
        <p>Olá, meu nome é Ana Lluiza Oliveira do Nascimento, moro em Camacari e estudo no SENAI, tenho 17 anos.
        Essa é minha página feita em HTML5.</p>

        <h2>Meu formulário</h2>

        <form>
            Nome:<br>
            <input type="text" value="Ana Lluiza Oliveira do Nascimento">
            <br><br>

            E-mail:<br>
            <input type="email" value="ana.l.nascimento8@ba.estudante.senai.br">
            <br><br>

            <button type="submit">Enviar</button>
        </form>
    </main>

    <footer>
        <p>Ana Lluiza Oliveira do Nascimento</p>
    </footer>

</body>
</html>

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
ATIVIDADE QUESTÂO 02 (CSS3 — Estilização de Cartão de Perfil)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# HTML 

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Meu cartão</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="cartao">

        <h1>Meu cartão ♡</h1>

        <img src="shih-tzu.jpg" alt="Cachorrinho Shih-tzu">

        <h2>Ana Luiza</h2>

        <p>Olá! Seja bem-vindo ao meu cartâo 2026!</p>

        <h3>Sobre mim</h3>
        <p>
            Sou uma estudante do - 2 ANO do ensino médio.
        </p>

        <h3>Minhas preferências</h3>
        <p>♡ Minha cor favorita: Rosa e ciano</p>
        <p>♡ Amo viajar e conhecer lugares novos.</p>
        <p>♡ Já conheci o Chile!</p>
        <p>♡ Meu animal favorito: Shih-tzu</p>
        <p>♡ Meu aniversário: 31 de outubro de 2009</p>

        <p class="final">
            momentos que fazem parte da minha história! ♡ :)
        </p>

    </div>

</body>
</html>

ATIVIDADE QUESTÂO 03 (CSS3 - Layout Responsivo com Flexbox ou Grid)
HTML

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Um pouco sobre mim</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Um pouco sobre mim ( ANALU ) ♡</h1>

    <p>Conheça algumas coisas que fazem parte da minha vida!</p>

    <div class="container">

        <div class="card">
            <h2>🌷 Sobre mim</h2>
            <p>Meu nome é Ana Luiza e nasci no dia 31 de outubro de 2009. Gosto de aproveitar os momentos especiais e guardar boas lembranças.</p>
        </div>

        <div class="card">
            <h2>AMOOOOO Viagens</h2>
            <p>Uma das coisas que mais gosto é viajar, conhecer lugares novos e descobrir outras culturas. Já tive a oportunidade de conhecer o Chile NO MEU ANIVERSARIO DE XV!!</p>
        </div>

        <div class="card">
            <h2>🐶 Coisas que EU amo</h2>
            <p>Gosto de MUITO de cachorros, principalmente da raça Shih-tzu, tenho dois. Gosto de fotografias e momentos com pessoas especiais ( MINHA FÁMILIA).</p>
        </div>

    </div>

</body>
</html>

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# CSS


body {
    font-family: Arial, sans-serif;
    background-color: #fceef2;
    text-align: center;
    margin: 0;
    padding: 30px;
}

h1 {
    color: #bd718c;
}

p {
    color: #555;
}

.container {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-top: 30px;
}

.card {
    background-color: white;
    padding: 20px;
    width: 250px;
    border-radius: 12px;
    box-shadow: 2px 3px 8px #d8bfc7;
}

.card h2 {
    color: #bd718c;
}

.card p {
    line-height: 1.5;
}

@media (max-width: 700px) {
    .container {
        flex-direction: column;
        align-items: center;
    }
}
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
ATIVIDADE QUESTÂO 04 (JavaScript - Manipulação do DOM e Evento de Clique)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# HTML

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Botão</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Bem-vindo!</h1>

    <p id="texto">Você está fora.</p>

    <button id="botao">Entrar</button>

    <script>
        document.getElementById("botao").addEventListener("click", function() {
            document.getElementById("texto").innerText = "Você entrou!";
        });
    </script>

</body>
</html>
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# CSS

body {
    background-color: #f2f2f2;
    font-family: Arial;
    text-align: center;
    margin-top: 100px;
}

button {
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
ATIVIDADE QUESTÂO 05 (JavaScript - Lógica Condicional e Validação Simples)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html>
<head>
    <title>Atividade</title>
</head>
<body>

    <h2>Verificar número</h2>

    <input type="number" id="numero">

    <button onclick="verificar()">Verificar</button>

    <p id="resultado"></p>

    <script>
        function verificar() {
            let n = document.getElementById("numero").value;

            if (n == "") {
                document.getElementById("resultado").innerText = "Digite um número";
            } else if (n % 2 == 0) {
                document.getElementById("resultado").innerText = "É par";
            } else {
                document.getElementById("resultado").innerText = "É ímpar";
            }
        }
    </script>

</body>
</html>

