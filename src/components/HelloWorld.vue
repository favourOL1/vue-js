<script setup>
import { ref } from 'vue'
import ClassBinding from './ClassBinding.vue';
import ForBinding from './ForBinding.vue';
import Event from './Event.vue';

defineProps({
  msg: String,
  head: String,
  

})

const count = ref(0)

const currentId= "Id-01"

const isButtonDisabled=false

const seen=true

const clicked= ()=>{
  alert('clicked')
}


</script>

<template>
  
  <Event/>

  <ForBinding/>

  <ClassBinding/>

  <h1  :id="currentId">{{ msg }}</h1>

  <h1>{{ head }}</h1>

  <p v-if="seen">Now you see me</p>

  <button v-on:click="clicked":disabled="isButtonDisabled">Button</button>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p>
  <p class="read-the-docs">Click on the Vite and Vue logos to learn more</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
