<script setup>
import logo from "@/assets/vue.svg";
</script>

<template>
  <header>
    <img :src="logo" alt="vue logo" />

    <h1>Hi, I'm <span class="highlight">Vue</span></h1>
  </header>
</template>

<style scoped>
header img {
  height: 150px;
}
header h1 {
  font-size: 2rem;
  color: #34495e;
  margin-top: 10px;
}
</style>
