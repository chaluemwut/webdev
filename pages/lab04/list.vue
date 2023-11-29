<template>
    <div>
        <div v-for="item in items">
            <span>{{ item.message }}</span>
        </div>

        <div>
            <button @click="addList">click</button>
        </div>
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import axios from 'axios'
const items = ref([{ message: 'aa' }, { message: 'bb' }])


onMounted(()=>{
    console.log('start page...')
})

</script>