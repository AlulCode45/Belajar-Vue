<script setup>
import { ref } from "vue";

const name = ref("Alul");

</script>


<template>
  <h1>Hello, {{ name }}🎉</h1>
</template>


<style scoped>
h1 {
  color: red;
}
</style>
