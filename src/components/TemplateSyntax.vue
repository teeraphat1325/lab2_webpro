<script setup>
var msg = 'Hello Message'
var rawHtml = '<h1>Hello</h1>'
var myId = 'myId1'
var color = 'blue'
var isDisable = true
var objectOfAttrs = {
  id: 'container',
  class: 'wrapper',
  style: 'background-color:green'
}
var number = 20
var ok = false
</script>

<template>
    <div>{{ msg }}</div>
    <div v-html="rawHtml"></div>
    <div v-bind:id="myId"></div>
    <font :color="color">Red</font>
    <button :disabled="isDisable">isEnable</button>
    <div v-bind="objectOfAttrs">Background Green</div>
    <div>{{ number +1 }}</div>
    <div>{{ ok ? 'Yes':'No' }}</div>
</template>