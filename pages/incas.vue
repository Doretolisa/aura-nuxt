<template>
  <div>
      <header>
        <div id="cabecalho1">
          <p class="stcabecalho1">PARCELE EM ATE 10X | CUPOM DE DESCONTO: BEAUTY253219</p>
        </div>
      </header>
      <nav>
        <div id="cabecalho2" class="stcabecalho2">
          <h1 class="logostyle">
            AURA
            <span style="font-family: 'Montserrat', sans-serif; font-size: 0.18em"
              >REALCE SUA BELEZA INTERIOR</span
            >
          </h1>
          <div class="search-container">
            <!-- Input com ícone de pesquisa -->
            <i class="fa fa-search"></i>
            <input
              type="text"
              style="padding-left: 30px; color: white"
              placeholder="Buscar Produto"
            />
          </div>
        </div>
      </nav>
      <hr style="margin: 0; border-top: 1.5px solid #000000" />
      <div class="video-container">
        <div class="cabecalho3">
          <a href="">TODOS OS PRODUTOS</a>
          <a href="">AURA SUMMER</a>
          <a href="">ROSTO</a>
          <a href="">CORPO</a>
          <a href="">MAQUIAGEM</a>
          <a href="">LOJAS</a>
        </div>

        <video class="video" width="70%" autoplay muted controls>
          <!-- <source src="AURA video.mp4" type="video/mp4" /> -->
        </video>
      </div>
  </div>
</template>
<style>
body,
header {
  margin: 0;
  padding: 0;
}
.stcabecalho1 {
  position: sticky; /* faz ele ficar fixo no topo da pagina */
  top: 0px;
  background-color: black;
  color: white;
  display: flex;
  justify-content: space-around;
  margin: 0;
}
.stcabecalho2 {
  position: static;
  margin: 0;
  background-color: rgb(120, 120, 225);
  display: flex;
  padding-top: 10px;
  justify-content: space-around;
}
.logostyle {
  font-family: "Hatton", sans-serif;
  color: white;
  font-size: 4rem;
}

.search-container {
  /*define largura do container input*/
  position: relative;
  top: 30px;
  width: 300px; /* Tamanho do input */
}

.search-container input[type="text"] {
  /*define estilo do texto do input*/
  width: 100%; /* Espaço para o ícone */
  font-size: 16px;
  border: 2px solid #ccc;
  border-radius: 20px;
  border-color: white;
  background-color: rgb(120, 120, 225);
}

.search-container .fa-search {
  /*define estilo do icone do input*/
  position: absolute;
  top: 18%;
  left: 10px;
  transform: translateY(-50%);
  font-size: 18px;
  color: white;
}

input::placeholder {
  color: white; /* Cor cinza escuro */
}

.search-container input[type="text"]:focus {
  border-color: #ffffff;
}

a {
  color: black;
}
a:hover {
  color: rgb(120, 120, 225); /* Cor ao passar o mouse */
}
.cabecalho3 {
  display: flex;
  justify-content: space-evenly;
  margin-left: 30px;
  margin-right: 30px;
}
.video-container {
  position: relative;
  text-align: center;
}
.video {
  border-radius: 10px;
  margin-top: 15px;
}
/*Fontes usadas na pagina:*/
@font-face {
  font-family: "Hatton";
  src: url("fonts/Hatton-Medium.otf") format("opentype");
}

@font-face {
  font-family: "Montserrat";
  src: url("fonts/Montserrat.ttf");
}
</style>
