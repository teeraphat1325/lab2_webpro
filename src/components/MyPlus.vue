<template>
    <div>
        <label for="num1"> num1</label>
        <input type="text" id="num1" v-model.number="num1">+
        <label for="num2"> num2</label>
        <input type="text" id="num2" v-model.number="num2">
        =
        {{  num1 + num2 }}
        <button>Calculate</button>
        {{ result }}
    </div>
</template>

<script setup>
import { ref } from 'vue'
const num1 = ref(0)
const num2 = ref(0)
const result = ref(0)
function Calculate() {
    result.value = num1.value + num2.value
}
</script>