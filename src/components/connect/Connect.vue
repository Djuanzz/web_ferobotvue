<template>
  <div class="connect-popup" v-if="isOpen">
    <div class="connect-content">
      <h1>Connect</h1>
      <input type="text" placeholder="IP Address" class="connect-input" />
      <button class="connect-button">Connect</button>
    </div>
  </div>
</template>

<script>
import "./connect.css";
import { ref } from "vue";

export default {
  name: "Connect",
  props: {
    isOpen: Boolean,
  },
};
</script>
