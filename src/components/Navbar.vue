
<template>
<div>
  <nav>
    <router-link to="/" class="nav-item" id="imagem"><Icone /></router-link>
      <div class="nav-list" @click="scrollToTop()">
      <router-link to="/" class="nav-item">Home</router-link>
      <router-link to="/locavorismo" class="nav-item">Locavorismo</router-link>
      <router-link to="/Produtores" class="nav-item"> Produtores </router-link>
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
  },
  methods: {
  scrollToTop() {
    window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
    }
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
  height: 70px;
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
  display: block;
    color: white;
    margin: 5px;
    padding: 5px;
    text-decoration: none;
  text-transform: uppercase;
  font-weight: bold;
  text-decoration: none;
  justify-content: space-around;
  transition: all 0.3s ease-in-out;
}
.nav-item:hover{
  transform: scale(1.1  );
  color: #896b35;
}
.nav-item.router-link-active {
  color: #004657;
}
.nav-item.router-link-active:hover{
  transform: scale(1.1);
}

@media (max-width: 768px) {
  nav {
    flex-direction: row;
    align-items: stretch;
    padding: 20px;
    position: relative;
  }
  #imagem{
    margin-top: 50px;
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
