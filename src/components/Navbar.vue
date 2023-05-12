<!--<template>
  <div id="nav">
   
      <router-link to="/" class="nav-item" id="imagem"><Icone /></router-link>
      <div class="nav-list">
      <router-link to="/" class="nav-item">Home</router-link>
      <router-link to="/locavorismo" class="nav-item">Locavorismo</router-link>
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
background-color: #d08f15;
border-bottom: 5px solid #e1e1e1;
padding: 5px 40px;
display: flex;
align-items: center;
height: 60px;
font-family: 'Gogh', sans-serif;
z-index: 99;
position: fixed;
  top: 0;
  left: 0;
  right: 0;
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
  color: #896b35;
}
.nav-item.router-link-active {
  color: #004657;
  transform: scale(1.1);
}
.nav-item.router-link-active:hover{
  transform: scale(1.2);
}
@media (max-width: 768px) {
  nav {
    flex-direction: column;
    align-items: stretch;
    padding: 20px;
  }

.nav-list {
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .nav-item {
    margin: 0 0 10px 0;
  }
}

</style>
-->

<template>
<div>
  <nav>
    <router-link to="/" class="nav-item" id="imagem"><Icone /></router-link>
      <div class="nav-list">
      <router-link to="/" class="nav-item">Home</router-link>
      <router-link to="/locavorismo" class="nav-item">Locavorismo</router-link>
      <router-link to="/contact" class="nav-item"> Produtores </router-link>
      <router-link to="/contact" class="nav-item">Potencial turístico</router-link>
      </div>
  </nav>
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

<style>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #f17d00;
  color: #fff;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 99;
}

.nav-list {
  list-style: none;
  display: flex;
  justify-content: space-between;
}

.nav-item {
  color: #fff;
  text-decoration: none;
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
  color: #896b35;
}
.nav-item.router-link-active {
  color: #004657;
  transform: scale(1.1);
}
.nav-item.router-link-active:hover{
  transform: scale(1.2);
}

@media (max-width: 768px) {
  nav {
    flex-direction: column;
    align-items: stretch;
    padding: 20px;
    position: relative;
  }

  .nav-list {
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .nav-item {
    margin: 0 0 10px 0;
  }
}
</style>
