<template>
    <div>
        click me: {{ count }}
    </div>
    <div>
        <button @click="onClick">click 123</button>
    </div>
</template>

<script setup>
    import {ref} from 'vue'
    const count = ref(0)

    function onClick(){
        count.value++
    }
</script>