<script setup>
import { ref } from "vue";
import ComponentRegistration from "./components/ComponentRegistration.vue";
import PropsBasic from "./components/PropsBasic.vue";
import EmitsBasic from "./components/EmitsBasic.vue";
import ComponentVModel from "./components/ComponentVModel.vue";

// emits basic
const total = ref(0);
const addTotal = () => {
  total.value++;
};

</script>

<template>

  <!-- component registration -->
  <ComponentRegistration />

  <!-- props -->
  <PropsBasic name="Alul" />

  <!-- emits basic -->
  <span>Total : {{ total }}</span>
  <EmitsBasic @add-total="addTotal" />

  <!-- v-model -->
  <ComponentVModel />

</template>
