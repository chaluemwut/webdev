<template>
    <div>
        <button v-on:click="clickMe">btn 1</button>
        <button @click="clickMe">btn2</button>
    </div>

    <div>
        <input @keyup="clickMe"/>
    </div>
</template>

<script setup>

function clickMe(){
    console.log('click me...')
}
</script>