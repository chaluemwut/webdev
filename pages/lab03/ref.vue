<template>
    <div>
        {{ counter }}
    </div>

    <div>
        <button class="btn btn-primary" @click="increment">click</button>
    </div>
</template>

<script setup>
import { ref } from 'vue'
const counter = ref(0)

function increment() {
    counter.value++
}

</script>