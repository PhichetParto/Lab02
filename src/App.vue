<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import CalComponentVue from "./components/CalComponent.vue";
import HelloWordExample from "./components/HelloWordExample.vue";
import HandingUserInput from "./components/HandingUserInput.vue";
import AttributeBindings from "./components/AttributeBindings.vue";
import ConditionsAndLoops from "./components/ConditionAndLoops.vue";
</script>

<template>
  <div>
    <ConditionsAndLoops></ConditionsAndLoops>
    <br />
    <br />
    <AttributeBindings></AttributeBindings>
    <HandingUserInput></HandingUserInput>
    <CalComponentVue></CalComponentVue>
    <HelloWordExample></HelloWordExample>
  </div>
</template>

<style scoped></style>
