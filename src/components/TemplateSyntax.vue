<script setup>
var msg = 'Hello Message'
var rawHtml = '<h1>Hello</h1>'
var myId = 'myId1'
var color = 'blue'
</script>

<template>
    <div>{{ msg }}</div>
    <div v-html="rawHtml"></div>
    <div v-bind:id="myId"></div>
    <font :color="color">Red</font>
</template>