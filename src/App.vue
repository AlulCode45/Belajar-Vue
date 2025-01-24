<script setup>
import { ref } from "vue";
import ComponentRegistration from "./components/ComponentRegistration.vue";
import PropsBasic from "./components/PropsBasic.vue";
import EmitsBasic from "./components/EmitsBasic.vue";

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

</template>
