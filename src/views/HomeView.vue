<template>
<div>
  <section class="home">
    <div class="text">  
      <h1>Quem somos?</h1>
      <div class="imagem1">
        <img class="movimento" src="/img/Movimentos.png" alt="">
      </div>
    </div>
  </section>

  <div class="home2">
    <!--Gradiente invertido-->
      <div class="home-2-logo">
        <img class="imagem-logo" src="/img/LOGO.png" alt="">
      </div>
      <div class="text-2">
       <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut fugit assumenda non harum corrupti rem consequuntur natus omnis dolores. Distinctio excepturi asperiores sequi eius voluptatum id enim officiis rem quis.</p>
      </div>
      <div class="text-3">
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sapiente, quas! Facere dolorum quae incidunt doloribus, molestiae non error quo perspiciatis porro, quisquam distinctio perferendis debitis quaerat, provident tempore excepturi atque.</p>
      </div>  
      <div class="text-button">
        <p>Conheça o que é o Locavorismo</p>
      </div>
      <div class="home-2-button">
        <router-link to="/about"><button @click="scrollToTop()" class="button">Definições</button></router-link>
      </div>
  </div>
</div>
   
</template>

<script>

export default{
  name: 'HomeView',
  components:{
  },
    methods: {
  scrollToTop() {
    window.scrollTo(0, 0);
    }
  } 
}

</script>

<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
 width: 100%;
 z-index: 0;
 overflow-x: hidden;
}

@keyframes move {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100px);
  }
}

  .imagem1 img {
  animation: move 2s alternate infinite;
  animation-timing-function: ease-in-out; 
  position: absolute;
  top: -90px;
  left: 170px;
  width: 70%;
  height: 80%;
  z-index: 1;
  
}

.home{
  background-image: url('../../public/img/gradiente.png');
  height: 120vh;
  background-repeat: no-repeat;
  background-size:cover ;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow-y: hidden;
  z-index: 0;
  position: relative;
}
.home2{
  background-image: url('../../public/img/gradiente2.png');
  width: 100%;
  height: 100vh;
  background-repeat: no-repeat;
  background-size:cover ;
  display: flex;
  align-items: center;
  justify-content: space-around;
  overflow-y: hidden;
  z-index:0 ;
  
}
.home2 img{
  position: absolute;
  display: flex;
  margin-top: -800px ;
  margin-left: 100px;
}
.imagem-logo{
  width: 500px;
  height: auto;
  padding: 2px 10px;
}
.text{
    font-size: 50px;
    font-family: 'Century Gothic';
    margin-top: -250px;
  }
.text-2{
  position: absolute;
  font-size: 30px;
  width: 600px;
  margin-top: -900px ;
  margin-left: 700px ;
  display: flex;
  justify-content: space-between;
  text-align: justify;
}
.text-3{
  position: absolute;
  font-size: 30px;
  display: flex;
  margin-top: -300px;
}
.text-button{
  white-space: nowrap;
  width: 100%;
  font-size: 40px;
  font-family: 'Century Gothic';
  margin-left: -250px;
  margin-top: 250px;
  background-color: red;
}
.button{
  width: 300px;
  background-color: transparent;
  border-radius: 20px;
  color: #000;
  cursor: pointer;
  padding: 6px 0;
  font-size: 20px;
  margin-top: 250px;
  
  transition: all 0.3s ease-in-out;
}
.button:hover{
  background-color: #ffffff;
  color: #21be5e;
}

</style>
