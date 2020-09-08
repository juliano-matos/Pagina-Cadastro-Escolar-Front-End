# Pagina-Cadastro-Escolar-Front-End
Pagina-Cadastro-Escolar-Front-End
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">

    <title>SWVSoftware</title>
  </head>
  
  <style>

    body{
        background:rgba(255, 255, 255, 0);
        font: normal 18pt Arial;
        margin: auto;
        }
        
        
        section {
        background-color:rgb(195, 197, 199);
        border-radius: 9px;
        padding: 18px;
        width: 936px;
        margin:auto;
        box-shadow: 1.3px 1.3px 1.3px rgba(0, 0, 0, 0.363);
        margin-block-start:0.6%;
        }

        #texto01 {
        background-color:rgb(146, 197, 255);
        }

        #alunocad {
        background-color: rgb(146, 197, 255);
        }
        
        #turmacad {
        background-color: rgb(146, 197, 255);
        }

        #myTab {
          text-decoration-color: black;
          background: linear-gradient(135deg, #051f2b 0%, #8efff0 99%);
        }
    
      </style>
      
  <body>
    <!--Div root ligação com os arquivos .JS-->
    
    <div id="root"></div>

    <ul class="nav nav-tabs" id="myTab" role="tablist">
        <li class="nav-item" role="presentation">
          <a class="nav-link active" id="home-tab" data-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true"><b>Home</b></a>
        </li>
        <li class="nav-item" role="presentation">
          <a class="nav-link" id="alunos-tab" data-toggle="tab" href="#alunos" role="tab" aria-controls="alunos" aria-selected="false"><b>Alunos</b></a>
        </li>
        <li class="nav-item" role="presentation">
          <a class="nav-link" id="turmas-tab" data-toggle="tab" href="#turmas" role="tab" aria-controls="turmas" aria-selected="false"><b>Turmas</b></a>
        </li>
      </ul>
      <div class="tab-content" id="myTabContent">
        <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">
          
          <section id='texto01'>
          <div>
            </div>
          <div>
            <h1><big><b>Olá,</b></big></h1>Este sistema foi desenvolvido para facilitar parte da administração de sua <br>
            escola e estamos felizes em ter você aqui!<br>
            <br>
            <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
            Saiba Mais...
          </button> <br>
        </div>
      </section>
          
    <section>
      <p>
              <!-- Button trigger modal -->
          
              <form>
                <div class="row">
                  <div class="col">
                    
                    <input type="text" class="form-control" placeholder="Procuras por...">
                  </div>

                </div>
              </form>

              <select class="form-control">
                <option>Aluno</option>
                <option>Turma</option>
              </select>
              <br>
              <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
              Pesquisar...
            </button>
          </section>

          </p>

          <section>
          <p>
            <h2><b>Alunos</b></h2>
            <p>Gerencie os alunos de uma forma fácil, cadastre, <br> edite e pesquise com poucos clicks! 
              <br>
              <button type="button" name='gerenciaral' id='gerenciaral' class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
              Gerenciar Alunos
            </button></p>
          </p>
          </section>

          <section>
          <p>
            <h2><b>Turmas</b></h2>
          
            <p>Gerencie as turmas de uma forma fácil, cadastre, <br> edite e pesquise com poucos clicks!

              <br>
              <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
              Gerenciar Turmas
            </button></p>
          </p>
               </section> </div> 
              </section>
       
          <div class="tab-pane fade" id="alunos" role="tabpanel" aria-labelledby="alunos-tab"><form>

            <h1><b><big>/ Alunos</big></b></h1>
            <section id='alunocad'>
           <p><h2><b>Cadastrar Aluno</b></h2></p>

          <form>
            <div class="row">
              <div class="col">
                <input name="nomealuno" id="nomealuno" min="0" type="text" class="form-control" placeholder="Nome Completo">
              </div>
              <div class="col">
                <input name="data" type="date" class="form-control" placeholder="Data de Nascimento">
              </div>
            </div>
          </form>

          <select name="Sexo" class="form-control">
            <option>Feminino</option>
          <option>Masculino</option>
          </select>
          <div class="col">
            <input name="Turma" type="text" class="form-control" placeholder="Ex:Turma01">
          </div>
          
          <br>
          <button type="button" name=cadAluno id="cadAluno" value="CadastrarAluno" onclick="cadAluno()" class="btn btn-success" data-toggle="modal" data-target="#exampleModal">
          Cadastrar
        </button><br>
      </section>

        <section>
      <p><h2><b>Pesquisar Alunos</b></h2></p>

        <form>
          <div class="row">
            <div class="col">
              <input name="Aluno" type="text" class="form-control" placeholder="Nome Completo">
            </div>
            
          </div>
        </form>

        <select name="Sexo" class="form-control">
          <option>Feminino</option>
          <option>Masculino</option>
        </select>

        <div class="col">
          <input name="Turma" type="text" class="form-control" placeholder="Ex:Turma02">
        </div>
        
        <br>
        <button type="submit" name=pesquisarAluno class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
        Pesquisar
      </button>
    </section>
</form></div>
            
<div class="tab-pane fade" id="turmas" role="tabpanel" aria-labelledby="turmas-tab"><form class="needs-validation" novalidate>
    
  <h1><b><big>/ Turmas</big></b></h1>
  <section id='turmacad'>
  <p><h2><b>Cadastrar Turma</b></h2></p>

          <form>
            <div class="row">
              <div class="col">
                <input name="Turma" type="text" class="form-control" placeholder="Descrição Turma">
              </div>
            </div>
          </form>
          <br>
          <button type="button" name="cadTurma" class="btn btn-success" data-toggle="modal" data-target="#exampleModal">
          Cadastrar
        </button> 
        </section>
  
        <section>
        <p><h2><b>Pesquisar Turma</b></h2></p>

        <form>
          <div class="row">
            <div class="col">
              <input name="Turma" type="text" class="form-control" placeholder="Turma">
            </div>
            
          </div>
        </form>
        <br>
        <button type="submit" name="pesquisarTurma" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
        Pesquisar 
      </button>
      </section>

    
      <section>
      <p> <h3><b>Visualizar Turmas</b></h3>  
        <br>
        <button name="visualizarTurma" type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
        Exibir
      </button>
    </section>
    </p>
        </form>
        
        <script>
        // Example starter JavaScript for disabling form submissions if there are invalid fields
        (function() {
          'use strict';
          window.addEventListener('load', function() {
            // Fetch all the forms we want to apply custom Bootstrap validation styles to
            var forms = document.getElementsByClassName('needs-validation');
            // Loop over them and prevent submission
            var validation = Array.prototype.filter.call(forms, function(form) {
              form.addEventListener('submit', function(event) {
                if (form.checkValidity() === false) {
                  event.preventDefault();
                  event.stopPropagation();
                }
                form.classList.add('was-validated');
              }, false);
            });
          }, false);
        })();
        </script></div>
      </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
    
  </body>
</html>
