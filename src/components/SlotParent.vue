<script setup lang="ts">
import { onMounted, ref } from 'vue'
import SlotChild from './SlotChild.vue'

const parentContent = ref<any>(null)

onMounted(() => {
  setTimeout(() => {
    parentContent.value = 'Parent Content'
  }, 2000)
})
</script>

<template>
  <h1>Slot</h1>
  <SlotChild>{{ parentContent }}</SlotChild>
</template>
