<script setup>
import { ref } from 'vue'


const text = ref ("")
const password = ref ("")
const username = ref ("")
const check = ref(false)
const selected = ref ("")





</script>


<template>

  <input v-model="text">

  <input type="username" v-model="username">

  <input type="password" v-model="password" >

  <input type="checkbox" v-model="check">

  <div> Selected: {{ selected }} </div>

  <select v-model="selected">

    <option disabled value=""> Please Select and Option</option>
    <option value="A">A</option>
    <option value="B">B</option>
    <option value="C">C</option>
    <option value="D">D</option>

  </select>



  <button @click="console.log(text, username, password, check, selected )" > SHOW </button>




</template>

<style scoped>

*{
  display: block;

}

input{
  height: 50px;
  
}



</style>
