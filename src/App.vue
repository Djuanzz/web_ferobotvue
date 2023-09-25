<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import ROSLIB from "../node_modules/roslib";
import Home from "./components/home/Home.vue";
import Navbar from "./components/navbar/Navbar.vue";
import Feature from "./components/feature/Feature.vue";
// import Connect from "./components/connect/Connect.vue";
</script>

<template>
  <!-- <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" /> -->

  <!-- <Connect /> -->
  <Navbar />
  <Home />
  <Feature />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
