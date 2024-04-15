<script setup>
import {ref} from 'vue'

defineProps({
    head:String,
    msg: String,

})

</script>


<template>

    <h1>
        {{ head }}
    </h1>

    <p>
        {{ msg }}
    </p>
</template>