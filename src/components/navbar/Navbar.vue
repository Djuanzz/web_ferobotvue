<template>
  <header class="navbar">
    <a href="#" class="nav-logo">Logoaku</a>

    <div class="nav-extra">
      <a href="#"><i class="fa-regular fa-user"></i></a>
      <a href="#feature"><i class="fa-regular fa-user"></i></a>
      <a href="#"><i class="fa-regular fa-user"></i></a>
      <a href="#"><i class="fa-regular fa-user"></i></a>
      <a href="#"><i class="fa-regular fa-user"></i></a>

      <div class="nav-status">
        <h4 class="status">Disconnected</h4>
        <!-- <a href="" id="connection" @click="isOpen = true"
          ><i class="fa-solid fa-link"></i
        ></a> -->
        <button @click="isOpen = true" class="nav-connect">
          <i class="fa-solid fa-link"></i>
        </button>
      </div>

      <div class="connect-content" v-if="isOpen">
        <h1>Connect</h1>
        <input type="text" placeholder="IP Address" class="connect-input" />
        <button type="submit" class="connect-button" @click="isOpen = false">
          Connect
        </button>
      </div>
    </div>
  </header>
</template>

<script>
import "./navbar.css";

import { ref } from "vue";
export default {
  name: "Navbar",
  setup() {
    const isOpen = ref(false);

    return {
      isOpen,
    };
  },
};
</script>
