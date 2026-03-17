# Olá 👋

<DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Linka o HTML e o CSS, permitindo a estilização mesmo que escrita em outro arquivo-->
    <link rel="stylesheet" href="Css.css">

    <!-- Título do site-->
    <title>Aula 1 HTML - Sistema escolar</title>

</head>
<body>

    <!-- Uma caixa para guardar informações, nesse caso, algumas frases -->
    <div id="titulo">
    <!-- O título NA pasta, basicamente, ele fará as letras terem o maior tamanho -->
    <h1>EEB Dom Jaime de Barros Câmara</h1>

    <p>Preencha o formulário para cadastrar um novo aluno</p>
    </div>

    <div id="caixaDePreencher">
    <form id="caixaDeCadastro">
        <label for="nome" class="preenchimento">Nome:</label>
        <input type="text" id="nome" name="nome"><br><br>

        <label for="dataNasc" class="preenchimento">Data de Nascimento: </label>
        <input type="date" id="dataNasc" name="dataNasc"><br><br>

        <label for="cpf" class="preenchimento">CPF: </label>
        <input type="text" id="cpf" name="cpf"><br><br>

        <label for="email" class="preenchimento">Email: </label>
        <input type="text" id="email" name="email"><br><br>

        <button type="button" class="cadastrar" onclick="mostrarDados()">Cadastrar</button>

    </form>
    </div>

        
        <div id="posicaoDoResultado"><div id="resultado">Vazio</div></div>

    
    <script>

        function mostrarDados(){

            let nome = document.getElementById("nome").value;
            let dataNasc = document.getElementById("dataNasc").value;
            let cpf = document.getElementById("cpf").value;
            let email = document.getElementById("email").value;

            // alert(nome + dataNasc + cpf + email)

            document.getElementById("resultado").innerHTML = 
            "Nome: " + nome + "<br>" +
            "Data de Nascimento: " + dataNasc + "<br>" +
            "CPF: " + cpf + "<br>" +
            "Email: " + email;


        }





    </script>

</body>
</html>
