<template>
<div class="home">
    <div class="home-logo">
      <img class="imagem-logo" src="/img/logo.png" alt="">
    </div>
    <div class="text">  
       <h1>Quem somos?</h1>
     </div>

     <div class="text-1">
      <p>O projeto denominado “Saberes e Sabores: Uma (re)visita ao interior” visa promover e explorar os conceitos de Locavorismo e Turismo Rural na nossa região, com foco principal no Maciço de Baturité. No entanto, pretendemos desenvolver métodos que possam ser efetivados em outras áreas, conforme o princípio da replicabilidade.
      </p>
      </div>
      <div class="text-2">
      <p>Nosso objetivo é promover o Locavorismo na região e aprofundar os laços sociais e culturais compartilhados entre produtores locais, consumidores e turistas. 
      </p>
      </div>
      <div class="text-3">
      <p>Nesse contexto, examinaremos de que forma se desenvolve a confiança, comunicação e cooperação nesta cadeia de produção, além de buscarmos disseminar estes saberes populares de uma forma educacional.
      </p>
      </div>
      <div class="text-4">
      <p>
        Deste modo, este estudo de caso se torna importante para verificar como o locavorismo busca explorar de forma sustentável os benefícios do turismo rural e dessa prática específica na economia local, bem como a renda que gera para os envolvidos no setor.
      </p>
      </div>
      <div class="text-button">
        <p>Conheça o que é o Locavorismo!</p>
        
      </div>
      <div class="home-2-button">
        <router-link to="/Locavorismo"><button @click="scrollToTop()" class="button">Clicando aqui!</button></router-link>
      </div>
</div>
<!--
      <div class="text-button">
        <p>Conheça o que é o Locavorismo</p>
      </div>
      <div class="home-2-button">
        <router-link to="/about"><button @click="scrollToTop()" class="button">Definições</button></router-link>
      </div>
  </div>

</div>
   -->
</template>

<script>
export default{
  name: 'HomeView',
  components:{
  },
    methods: {
  scrollToTop() {
    this.$router.push('/Locavorismo');
    }
  } 
}

</script>

<style scoped>
*{
  margin: 0;
  margin-top: 30px;
  padding: 0;
  box-sizing: border-box;
 width: 100%;
 z-index: 0;
 overflow-x: hidden;
}

.home{
  background-color: #ffa600;
  background-image: url('../../public/img/Desfocado.png');
  height: 400vh;
  background-repeat: no-repeat;
  background-size:cover ;
  display: block;
  align-items: center;
  justify-content: center;
  overflow-y: hidden;
  z-index: 0;
  position: relative;
}
.home{
  background-image: url('../../public/img/Desfocado.png') 
}
.home-logo{
  padding: 20px;
}

.imagem-logo{
  width: 500px;
  height: auto;
  padding: 2px 10px;
}
.text{
    font-size: 50px;
    font-family: 'Century Gothic';
  }
  .text-1{
  position: relative;
  font-size: 30px;
  width:500px;
  margin-top: 90px ;
  margin-left: 700px ;
  display: flex;
  justify-content: space-between;
  text-align: justify;
}
.text-2{
  position: relative;
  font-size: 30px;
  width: 600px;
  margin-top: 90px ;
  display: flex;
  justify-content: space-between;
  text-align: justify;
}
.text-3{
  position: relative;
  font-size: 30px;
  width:500px;
  margin-top: 90px ;
  margin-left: 700px ;
  display: flex;
  justify-content: space-between;
  text-align: justify;
}
.text-4{
  position: relative;
  font-size: 30px;
  width:500px;
  margin-top: 90px ;
  margin-left: 700px ;
  display: flex;
  justify-content: space-between;
  text-align: justify;
}
.text-button {
  width: 100%;
  height: auto;
  margin-top: 350px;
  margin-left: 450px;
}
.text-button p{
  width: 100%;
  height: auto;
  display: flex;
  font-size: 38px;
  font-family: 'Century Gothic';
}
.button{
  background-color: transparent;
  border: 2px solid #000;
  color: #000;
  padding: 10px 20px;
  width: 300px;
  font-size: 16px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  border-radius: 20px;
  transition: all 0.3s ease;
}
.button:hover{
  background-color: #ffffff;
  color: #21be5e;
}

@media (max-width: 768px) {
  
}
</style>
