<script setup lang="ts">
const props = defineProps({
  msg: String
})
</script>

<template>
  <h3>Value from parent: {{ props.msg }}</h3>
</template>
