<template>
  <section class="home">
    <div class="home-content">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione,
        maiores.
      </p>
      <div class="connect-content" v-if="isOpen">
        <h1>Connect</h1>
        <input type="text" placeholder="IP Address" class="connect-input" />
        <button class="connect-button" @click="isOpen = false">Connect</button>
      </div>
    </div>
  </section>
</template>

<script>
import "./home.css";

export default {
  name: "Home",
};
</script>
