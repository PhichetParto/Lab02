<script setup lang="ts">
import { ref } from "vue";
const show = ref(true);
const list = ref([1, 2, 3]);
</script>

<template>
  <button @click="show = !show">Toggle List</button>
  <button @click="list.push(list.length + 1)">Push Number</button>
  <button @click="list.pop()">Pop Number</button>
  <button @click="list = list.reverse()">Reverse List</button>

  <u1 v-if="show && list.length">
    <li v-for="(item, index) of list" :key="index">{{ item }}</li>
  </u1>
  <p v-else-if="list.length">List is not empty, but hidden.</p>
  <p v-else>List is empty</p>
</template>

<style scoped></style>
