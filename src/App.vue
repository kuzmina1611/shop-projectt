<template>
  <div id="app">
    <ClothingBlock />
  </div>
</template>

<script setup>
import ClothingBlock from './components/ClothingBlock.vue'
</script>

<style>
html, body {
  margin: 0;
  padding: 0;
  background: white;
}

#app {
  font-family: Arial, sans-serif;
  padding: 0;
  background: white;
  min-height: 100vh;
}
</style>