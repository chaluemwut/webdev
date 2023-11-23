<template>
    <div>
        {{ counter.a }}
    </div>
    <div>
        <button @click="increment">click</button>
    </div>
</template>

<script setup>
import { ref } from 'vue'
const counter = ref({ m: { 'k1': 10, 'k2': 20 }, a: ['a', 'b'] })

function increment() {
    counter.value.a.push('c')
}

</script>