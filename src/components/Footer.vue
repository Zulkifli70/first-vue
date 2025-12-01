<template>
  <footer>
    <p>
      Learn more about me at
      <a target="_blank" :href="link">vuejs.org</a>
    </p>
    <button :disabled="isBtnDisabled">Another!</button>
    <button v-bind:disabled="isBtnDisabled">Share</button>
  </footer>
</template>

<script setup>
import { ref } from "vue";
const link = ref("https://vuejs.org/");

const isBtnDisabled = ref(true);
</script>

<style scoped>
footer {
  margin-top: 35px;
  font-size: 0.8rem;
}

footer a {
  color: #40b883;
}

button {
  background: #406473;
  color: white;
  padding: 10px;
  border: 0;
  font-size: 1.2rem;
  border-radius: 0 5px 0 5px;
  font-weight: bold;
  margin-top: 20px;
  cursor: pointer;
  transition: transform 0.2s;
}
button:hover {
  transform: scale(1.05);
}
button:disabled {
  background: grey;
  cursor: not-allowed;
  opacity: 0.5;
}
</style>
