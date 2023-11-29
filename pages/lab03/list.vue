<template>
    <div v-for="data in l">
        {{ data }}
    </div>
</template>

<script setup>
import { ref } from 'vue'
const l = ref([1, 2, 3])
</script>