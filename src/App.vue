<script setup>
import Hello from './components/HelloComponent.vue'
import TemplateSyntax from './components/TemplateSyntax.vue'
import ReactiveFundamentals from './components/ReactivityFundamentals.vue'
import FormInputBindings from './components/FormInputBindings.vue'
</script>

<template>
  <FormInputBindings></FormInputBindings>
  <hr>
  <ReactiveFundamentals></ReactiveFundamentals>
  <hr>
  <div>Hello</div>
  <hr>
  <span><Hello></Hello></span>
  <hr>
  <TemplateSyntax></TemplateSyntax>
  <hr>
</template>

<style scoped>

</style>
