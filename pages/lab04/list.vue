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
import { ref } from 'vue'
const items = ref([{ message: 'aa' }, { message: 'bb' }])

function addList() {
    items.value.push({ message: 'ddd' })
}

</script>