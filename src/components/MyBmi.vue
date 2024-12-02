<template>
    <div>
        <label for="weight">น้ำหนัก</label>
        <input type="text" id="weight" v-model.number="weight"> kg.
        <br>   
        <label for="height">ส่วนสูง</label>
        <input type="text" id="height" v-model.number="height"> cm.
        <br>
        {{ weight }} {{ height }}
        <br>
        <button @click="calBmi()">Cal BMI</button>
        <br>
        BMI = {{ result }}
    </div>
</template>

<script setup>
import { ref } from 'vue'
const weight = ref(0)
const height = ref(0)
const result = ref(0)
function calBmi() {
 result.value = weight.value / (height.value/100)**2
}
</script>