<script setup>
import Forms from './components/Forms.vue';
import HelloWorld from './components/HelloWorld.vue'
import MyComponent from './components/MyComponent.vue';
</script>

<template>
  <Forms/>
  <MyComponent msg="My first Vue Website" head="My name is Favour"/>
  <HelloWorld msg="Vite + Vue"  head="hello"/>
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
