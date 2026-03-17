<html>

<head>
    <title>Sistema Escolar</title>

</head>

</html>
<style>


    .titulo {

        font-size: 20px;
        color: rgb(255, 255, 255);
        margin-top: 70px;
        text-align: center;

    }

    .formulario {
        background-color: rgb(233, 169, 169);
        width: 600px;
        padding: 20px;
        border-radius: 8px;
        border: 2px solid black;
        margin: auto;
    }

    .cadastro {
        cursor: pointer;
        margin: auto;
        display: block;
    }
    #resultado{
        background-color: rgb(233, 169, 169);
        width: 600px;
        padding: 20px;
        border-radius: 8px;
        border: 2px;
        margin: auto;
        margin-top: 90px;
    }



</style>




<body>

    <div class="titulo">

        <h1>EEB Dom Jaime de Barros Câmara</h1>

        <p>Preencha o formulário abaixo para cadastrar um novo aluno</p>



    </div>
    <div class="formulario">

        <from>

            <label for="nome">Nome:</label><br>
            <input type="text" id="nome" name="nome"><br><br>

            <label for="dataNasc">Data de Nascimento<label>
            <input type="date" id="dataNasc" name="dataNasc"><br><br>
            <label for="cpf">CPF</label><br>
            <input type="text" id="cpf"><br>

            <label for="email">Email: </label><br>
            <input type="text" id="email" name="email"><br><br>



            <button type="button" class="cadastrar" onclick="mostrarDados()">Cadastrar</button>







        </from>


    </div>

    <div id="resultado">



    </div>


    <script>
        function mostrarDados() {
            let nome = document.getElementById("nome").value
            let dataNasc = document.getElementById("dataNasc").value
            let cpf = document.getElementById("cpf").value
            let email = document.getElementById("email").value

            let resultado = document.getElementById("resultado")

            document.getElementById("resultado").innerHTML = "<h2>Dados Informados: <h2>" +
                "Nome: " + nome + "<br>" +
                "Data de Nascimento: " + dataNasc + "<br>" +
                "CPF: " + cpf + "<br>" +
                "Email:" + email;
                
                resultado.style.display = "block"
                
        }





    </script>






</body>

</html>
