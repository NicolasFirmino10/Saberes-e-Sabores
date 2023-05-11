<template>
  <div id="nav">
   
      <router-link to="/" class="nav-item" id="imagem"><Icone /></router-link>
      <div class="nav-list">
      <router-link to="/" class="nav-item">Home</router-link>
      <router-link to="/about" class="nav-item">Locavorismo</router-link>
      <router-link to="/contact" class="nav-item"> Produtores </router-link>
      <router-link to="/contact" class="nav-item">Potencial turístico</router-link>

    </div>
   
</div>
</template>

<script>
import Icone from './Icone.vue'

export default {
  name: 'Navbar',
  components:{
    Icone
  }
}

</script>



<style scoped>

#nav{
background-color: #00a281;
border-bottom: 5px solid #e1e1e1;
padding: 5px 40px;
display: flex;
align-items: center;
height: 60px;
font-family: 'Gogh', sans-serif
}
#imagem{
  max-width: 30px;
  margin-right: 30px;
  height: auto;
  transform: scale(0.7); 
}

.nav-list {
  list-style: none;
  display: flex;
  margin-left: 800px;
  align-items: center;
  justify-content: space-between;
}

.nav-item {
  display: block;
    color: white;
    padding: 10px 12px;
    text-decoration: none;
  margin: 0 10px;
  text-transform: uppercase;
  font-weight: bold;
  letter-spacing: 1px;
  transition: all 0.3s ease-in-out;
}
.nav-item:hover{
  transform: scale(1.2);
}
.nav-item.router-link-active {
  color: #004657;
  transform: scale(1.1);
}
.nav-item.router-link-active:hover{
  transform: scale(1.2);
}

</style>
