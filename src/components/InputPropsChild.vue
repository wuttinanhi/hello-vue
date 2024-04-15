<script setup lang="ts">
const props = defineProps({
  msg: String
})
</script>

<template>
  <h3>Value from parent: {{ msg }}</h3>
</template>
