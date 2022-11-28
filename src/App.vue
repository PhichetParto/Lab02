<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponentVue from "./components/CalComponent.vue";
import HelloWordExample from "./components/HelloWordExample.vue";
</script>

<template>
  <div>
    <CalComponentVue></CalComponentVue>
    <HelloWordExample></HelloWordExample>
  </div>
</template>

<style scoped></style>
