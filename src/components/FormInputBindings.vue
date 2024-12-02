<template>
    <div>Form Input Bindings</div>
    <div>{{ text }}</div>
    <input v-model="text"/>

    <span>Multiline message is:</span>
    <p style="white-space: pre-line;">{{ message }}</p>
    <textarea v-model="message" placeholder="add multiple lines"></textarea>

    <input type="checkbox" id="checkbox" v-model="checked" />
    <label for="checkbox">{{ checked }}</label>

    <div>Checked names: {{ checkedNames }}</div>

    <input type="checkbox" id="jack" value="Jack" v-model="checkedNames" />
    <label for="jack">Jack</label>

    <input type="checkbox" id="john" value="John" v-model="checkedNames" />
    <label for="john">John</label>

    <input type="checkbox" id="mike" value="Mike" v-model="checkedNames" />
    <label for="mike">Mike</label>

    <div>Picked: {{ picked }}</div>

    <input type="radio" id="one" value="One" v-model="picked" />
    <label for="one">One</label>

    <input type="radio" id="two" value="Two" v-model="picked" />
    <label for="two">Two</label>

    <div>Selected: {{ selected }}</div>

    <select v-model="selected">
    <option disabled value="">Please select one</option>
    <option>A</option>
    <option>B</option>
    <option>C</option>
    </select>

    <div>Selected: {{ selected2 }}</div>

    <select v-model="selected2" multiple>
    <option>A</option>
    <option>B</option>
    <option>C</option>
    </select>
</template>

<script setup>
import { ref } from 'vue'
const text = ref('hello')
const message = ref('')
const checked = ref(true)
const checkedNames = ref([])
const picked = ref('')
const selected = ref('')
const selected2 = ref([])
</script>