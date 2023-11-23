<template>
    <div>
        c is {{ c }}
    </div>

    <div>
        <button class="btn btn-primary" @click="c++">click me</button>
    </div>
</template>

<script setup>
import {ref} from 'vue'

const c = ref(0)

</script>