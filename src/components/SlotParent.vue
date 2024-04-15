<script setup lang="ts">
import { onMounted, ref } from 'vue'

const parentContent = ref<any>(null)

onMounted(() => {
  setTimeout(() => {
    parentContent.value = 'Parent Content'
  }, 2000)
})
</script>

<template>
  <SlotChild>{{ parentContent }}</SlotChild>
</template>
