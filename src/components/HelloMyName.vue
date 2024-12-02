<template>
    <div>
        <input type="text" v-model="name">
        <div>Hello {{  name  }}</div>
        
    </div>
</template>

<script setup>
import { ref } from 'vue'
    const name = ref('')
</script>