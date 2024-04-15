<script setup lang="ts">
const emit = defineEmits(['myresponse'])

emit('myresponse', 'hello from child!')
</script>

<template>
  <h2>Child component emitting to parent</h2>
</template>
