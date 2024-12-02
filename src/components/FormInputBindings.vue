<template>
    <div>Form Input Bindings</div>
    <div>{{ text }}</div>
    <input type="text" :value="text" @input="(e) => (text = e.target.value)"/>
</template>

<script setup>
import { ref } from 'vue'
const text = ref('hello')
// const inputText =  (e) => (text.value = e.target.value)
</script>