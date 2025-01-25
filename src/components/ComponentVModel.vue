<script setup>
const username = defineModel('username')
const password = defineModel('password')
</script>

<template>
  <form action="">
    <input type="text" v-model="username" placeholder="Username" />
    <input type="password" v-model="password" placeholder="Password" />
  </form>

  <p>Username: {{ username }}</p>
  <p>Password: {{ password }}</p>
</template>
