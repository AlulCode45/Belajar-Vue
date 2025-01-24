<script setup>
defineEmits(['add-total'])
</script>



<template>
  <button @click="$emit('add-total')">Tambah</button>
</template>
