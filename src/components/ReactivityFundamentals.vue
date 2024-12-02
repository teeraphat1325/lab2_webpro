<template>
    <div>{{ count }}</div>
    <button @click="increment()">{{ count }}</button>

    <div>{{ state.count }}</div>
    <button @click="increment1()">{{ state.count }}</button>
</template>

<script setup>
import { ref , reactive } from 'vue'
const state = reactive({
    count: 0,

})
function increment1() {
    state.count++
}
const count = ref(0)
function increment() {
    count.value++
}
</script>
