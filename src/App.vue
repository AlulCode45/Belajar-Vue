<script setup>
import { ref } from "vue";
import ComponentRegistration from "./components/ComponentRegistration.vue";
import PropsBasic from "./components/PropsBasic.vue";
import EmitsBasic from "./components/EmitsBasic.vue";
import ComponentVModel from "./components/ComponentVModel.vue";
import InterpolationComponent from "./components/InterpolationComponent.vue";

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
  <div>
    <span>Total : {{ total }}</span>
    <EmitsBasic @add-total="addTotal" />
  </div>

  <br>
  <!-- v-model -->
  <ComponentVModel />

  <!-- v-text -->
  <InterpolationComponent />

</template>
