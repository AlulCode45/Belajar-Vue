<script setup>
import { ref } from 'vue';

const image = ref('https://picsum.photos/seed/picsum/536/354');
const usernameModel = defineModel('username');
const vOnce = ref("Some Text");

</script>
<template>

  <h1>MessageInterpolation</h1>

  <!-- vtext -->
  <p v-text="'Belajar'"></p>
  <!-- vhtml -->
  <p v-html="'<h1>belajar</h1>'"></p>
  <!-- vbind -->
  <img :src="image" alt="">
  <!-- vmodel -->
  <input type="text" v-model="usernameModel" placeholder="Username" />
  <p>Username: {{ usernameModel }}</p>
  <!-- vonce -->
  <input v-model="vOnce">
  <p v-once>{{ vOnce }}</p>
  <!-- vpre -->
  <p v-pre>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, natus reiciendis quibusdam eveniet obcaecati
    assumenda rerum amet soluta doloribus commodi in vero exercitationem qui delectus accusamus quaerat reprehenderit
    saepe ipsa.
  </p>
  <!-- vif -->
  <h1 v-if="true">Vue is awesome!</h1>
</template>
