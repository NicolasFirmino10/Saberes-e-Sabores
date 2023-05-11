<template>

  <div>
  <section class="about">
    <div class="text">
       <h1>Locavorismo</h1>
    </div>
  </section>
  <div class="imagem">
      <div class="foto">
        <img src="/img/matriz.png" alt="">
      </div>
    </div>
  <div class="about2">

  </div>
  </div>
</template>
  
  <script>

  export default{
    name: 'about',
    components:{
    }
  }
  
  </script>
  
  <style scoped>
  *{
    margin: 0;
   width: 100%;
   z-index: 0;
   overflow-x: hidden;
  }
  
  .about{
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
  .imagem img{
    display: flex;
   position: relative;
   left: 350px;
  width: 90%;
  height: 100%;
}
  .about2{
    background-image: url('../../public/img/gradiente2.png');
    height: 100vh;
    background-repeat: no-repeat;
    background-size:cover ;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow-y: hidden;
    z-index: 0;
    position: relative;
  }
  .foto{
    position: absolute;
  display: flex;
justify-content: space-around;  z-index: 99;
  margin-top: -250px;
  margin-right: -250px;
 
  }
  
  .text{
      width: 700px;
      font-size: 35px;
      text-align: justify;
      margin-right: 30px;
      margin-top: 20px;
      font-family: 'Century Gothic';
  
    }
    .text h1{
     
      width: 100%;
      display: flex;
      justify-content: center;
      font-family: 'Century Gothic';
      transition: font-size 0.3s ease-in-out;
    
    }
  </style>
  