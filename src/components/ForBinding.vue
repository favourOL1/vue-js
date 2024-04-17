<script setup>
import { ref } from 'vue'



const list = ["Apple", "Orange", "Banana", "Mango"]




</script>


<template>

    <ul>
        <li v-for="item in list " >

            {{ item }}

        </li>
    </ul>

   
</template>

<style scoped>



</style>
