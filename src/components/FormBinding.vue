<script setup lang="ts">
import { ref } from "vue";
const text = ref("Edint Me");
const checked = ref(true);
const checkedNames = ref(["Jack"]);
const picked = ref("One");
const selected = ref("A");
const multipleSelected = ref([""]);
</script>

<template>
  <h2>Text Input</h2>
  <input v-model="text" /> {{ text }}

  <h2>Checkbox</h2>
  <input type="checkbox" id="checkbox" v-model="checked" />
  <label for="checkbox">Checked: {{ checked }}</label>

  <h2>Multi Checkbox</h2>
  <input type="checkbox" id="jack" value="Jack" v-model="checkedNames">
  <label for="jack">Jack</label>
  <input type="checkbox" id="john" value="John" v-model="checkedNames">
  <label for="john">John</label>
  <input type="checkbox" id="mike" value="Mike" v-model="checkedNames">
  <label for="mike">Mike</label>
  <p>Checked names: <pre>{{ checkedNames }}</pre></p>

  <h2>Radio</h2>
  <input type="radio" id="one" value="One" v-model="picked" />
  <label for="one">One</label>
  <input type="radio" id="two" value="Two" v-model="picked" />
  <label for="two">Two</label><br />
  <span>Picked: {{ picked }}</span>

    <h2>Select</h2>
    <select v-model="selected">
    <option disabled value="">Please select one</option>
    <option value="1">A</option>
    <option value="2">B</option>
    <option value="3">C</option>
</select>
<span>Selected {{ selected }}</span>

<h2>Multiple Select</h2>
    <select v-model="multipleSelected" multiple style="width: 100px">
    <option disabled value="">Please select one</option>
    <option value="1">A</option>
    <option value="2">B</option>
    <option value="3">C</option>
</select>
<span>Multiple Selected {{ multipleSelected }}</span>

</template>
