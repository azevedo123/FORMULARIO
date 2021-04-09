<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario</title>
<style>
    *{
      margin:0;
      padding:0;
    }

    #titulo{
        font-family: sans-serif;
        color:lightblue;
        margin-left: 7%;
    }

    #subtitulo{
        font-family: sans-serif;
        color:lightblue;
        margin-left: 10%;
    }

    label{
          color:mediumturquoise;
    }

    fieldset{
             border: 10px;
    }

    body{
         background-color:lightcyan;
         font-family: sans-serif;
         font-size: 1em;
         color:olive;
         margin-left: 36%;
         margin-top: 2%;
         justify-content: center;
    }

    input, select, textarea, button{
        border-radius: 5px;
    }

    .campo{
        margin-bottom: 2em;
    }

    .campo label{
        margin-bottom: 0.2em;
        color:mediumturquoise;
        display: block;
    }

    fieldset.grupo .campo{
        float: left;
        margin-right: 3em;
    }

    .campo input[type="text"], .campo input[type="email"], .campo select, .campo textarea{
        padding: 0.2em;
        border: 1px solid rgba(3, 0, 0, 0.795);
        box-shadow: 2px 2px 2px #6495ED;
        display: block;
    }

    .campo select option{
        padding-right: 1em;
    }

    .campo input:focus, .campo select:focus, .campo textarea:focus{
        background:white;
    }

    .botao{
        font-size: 1.2em;
        background:cornsilk;
        border:0;
        color:brown;
        padding: 0.2em 0.6em;
        box-shadow: 2px 2px 2px #6495ED;
        text-shadow: 1px 1px 1px #0000;
        position: absolute;
        top: 90%;
        margin-right: -50%;
        transform: translate(-50%, -50%);
    }
    
    .botao:hover{
        background: rgb(7, 27, 48);
        box-shadow: inset 2px 2px 2px #87CEEB;
        text-shadow: none;

    }

    .botao, select{
        cursos:pointer;
    }

    #check{
        display: inline-block;
    }

</style>
</head>
<body>
     <div>
         <h1 id="titulo">Cadastro</h1>
         <p id="subtitulo"><strong>Complete suas informações</strong></p>
         <br>
     </div>
    
     <forms>
         <fieldset class="grupo">
             <div>
                <label for="nome"><strong>nome</strong></label>
                <input type="text" name="nome" id="nome" required>
             </div>
             
             <div class="campo">
                 <label for="sobrenome"><strong>sobrenome</strong></label>
                 <input type="text" namw="sobrenome" id="sobrenome" required>
             </div>
             <div>
                <label><strong>idade</strong></label>
                <label><input type="text" name="idade" id="idade" required></label>
            
            </fieldset>
       
         <div>
            <label><strong>email</strong></label>
            <input type="email" name="email" id="email" required>
        </div>
        
        <div class="campo">
            <label><strong>qual lado da aplicação vc é?</strong></label>
            <label>
                <input type="radio" name="deviweb" value="frontend"><strong>Front-end</strong>
            </label>
            <label>
                <input type="radio" name="deviweb"  value="backend"><strong>back-end</strong>
            </label>
            <label>
              <input type="radio" name="deviweb" value="fullstack"><strong>fullstack</strong>
            </label>
        </div>
       
        <div>
           <label><strong>Senerosidade</strong></label>
           <select id="senerosidade">
           <option select disabled value=""><strong>Selecione</strong></option>
           <option>junior</option>
           <option>pleno</option>
           <option>senior</option>
            </select>
        </div>

        <fieldset class="grupo">
            <div id="check">
                <label><strong>Selecione as informações abaixo</strong></label><br>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label for="tecnologia1">HTML</label>
                <input type="checkbox" id="tecnologia2"  name="tecnologia2" value="CSS">
                <label for="tecnologia2">CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="javacript">
                <label for="tecnologia3">javacript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="pip">
                <label for="tecnologia4">PIP</label>
            </div>
        </fieldset>

        <div class="campo">
            <br>
            <label><strong>Faça um resumo da sua experiencia</strong></label>      
          <textarea form="6" style="width: 26em" id="experiencia" name="experiencia"></textarea>
        </div>

        <boton class="botao" type="submit">Concluido</boton>
     </forms>

</body>
</html>

