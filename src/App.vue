<template>
  <img alt="Vue logo" class="element-plus-logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3.0 + Element Plus + Vite" />
</template>

<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--el-text-color-primary);
  background-color: var(--el-background-color-base);
}
.element-plus-logo {
  width: 50%;
}
</style>
