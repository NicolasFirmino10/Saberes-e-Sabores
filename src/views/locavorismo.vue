<template>
    <div class="home">
        
        <img class="imagem-local" src="/img/local.png" alt="">
        
        
    <div class="home-logo">
        <img class="imagem-logo" src="/img/locavorismo.png" alt="">
    </div>
        <div class="text">  
            <div class="text-1">
                 <p>Comprar e utilizar mercadorias de fontes locais ou estabelecimentos menores tornou-se uma prática conhecida como locavorismo. As cidades do interior abrigam as conhecidas "bodegas" que atendem a essa tendência. A palavra "locavorismo" é derivado de "local" e "-voro", uma palavra latina que significa "comer", ou seja, é o consumo mais sustentável de uma região. 
                 </p>
                 <img class="imagem-caju" src="/img/caju.png" alt="">
            </div>
            <div class="text-2">
                
                <img class="imagem-banana" src="/img/banana.png" alt="">
                <p>A preferência por esse tipo de uso está relacionada à praticidade e facilidade de disponibilidade dos produtos alimentícios e à busca de uma relação equilibrada com o meio ambiente. O locavorismo também busca evitar a perda de nutrientes, o frescor e o impacto ambiental que o alimento tem ao percorrer uma longa jornada até chegar ao mercado de massa.
                </p>
            </div>
            <div class="text-3">
                <img class="imagem-cafe" src="/img/cafe.png" alt="">
                <p>O termo, em seu sentido literal, refere apenas ao consumo de produtos do ramo alimentícios. Mas nós enquanto locávoros abrangemos o termo para o consumo de um território em suas mais diversas formas.
                </p>
            </div>
            <div class="text-4">
                <img class="imagem-carta" src="/img/carta.png" alt="">
            <p>
                O projeto Saberes e Sabores visa analisar e promover o Locavorismo de forma holística. Incentivando não somente o consumo de alimentos produzidos próximo aos consumidores, mas também a cultura, o turismo, a arte, a economia e a história da região.
            </p>
            </div>
        </div>
        <div class="text-button">
            <p>Agora, conheça um pouco dos nossos  produtores!</p>
        </div>
        <div>
            <router-link to="/Produtores"><button @click="scrollToTop()" class="button">Clicando aqui!</button></router-link>
        </div>
    </div>
</template>

<script>

export default{
    name: 'Locavorismo',
    methods: {
  scrollToTop() {
    this.$router.push('/Locavorismo');
    window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
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
.home{
    background-color: #EF8535;
    height: 360vh;
}
.imagem-logo{
    width: 500px;
    margin-top: 100px;
}
.imagem-cafe{
    position: absolute;
    width: 350px;
    margin-left: 500px;
    margin-top: -100px;
}
.imagem-local{
    position: absolute;
    width: 200px;
    margin-top: 600px;
    margin-left: -700px;
}
.imagem-caju{
    position: absolute;
    margin-left: -500px;
    width: 250px;
    margin-top: 100px;
}
.imagem-banana{
    position: absolute;
    width: 250px;
    margin-top: 150px;
    margin-left: -700px;
}
.imagem-carta{
    position: absolute;
    width: 300px;
    margin-top: 150px;
    margin-left: 700px;
}
.text-1{
    width: 700px; 
    margin-left: 260px ;
    margin-top: 100px;
    font-size: 32px;
}
.text-2 {
    width: 700px; 
    margin-left: 750px;
    margin-top: 100px;
    font-size: 32px;
  }
  .text-3{
    width: 650px;
    margin-left: 100px;
    margin-top: 200px;
    font-size: 33px;
  }
  .text-4{
  font-size: 32px;
  width:700px;
  margin-top: 150px ;
  margin-left: 400px;
  display: flex;
  text-align:unset; 
 }

 .text-button p{
  width: 500px;
  height: auto;
  display: flex;
  font-size: 38px;
  margin-left: 500px;
  margin-top: 100px;
  margin-bottom: 60px;
  text-align:center;
  font-family: 'Century Gothic';
}
  .button{
  background-color: transparent;
  border: 2px solid #000;
  color: #000;
  cursor: pointer;
  padding: 10px 20px;
  width: 300px;
  font-size: 18px;
  text-align: center;
  border-radius: 20px;
  transition: all 0.3s ease;
}
.button:hover{
  background-color: #ffffff;
  color: #6f5f17;
}

</style>