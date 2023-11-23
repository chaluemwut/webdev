<template>
    <div>
        {{ counter }}
    </div>

    <div>
        <button @click="counter++">click</button>
    </div>
</template>

<script setup>
import {ref} from 'vue'
const counter = ref(0)
counter.value++
console.log(counter.value)
</script>