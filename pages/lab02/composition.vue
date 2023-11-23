<script setup>
import { ref, onMounted } from 'vue'
import axios from 'axios'

const count = ref(0)

function increment() {
  count.value++
  console.log(count)
}

onMounted(() => {
  console.log(`The initial count is ${count.value}.`)
})

</script>

<template>
  <button @click="increment">Count is: {{ count }}</button>
</template>