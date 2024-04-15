<script setup lang="ts">
import { onMounted, ref } from 'vue'

const pElementRef = ref(null)
const delayedText = ref('')

onMounted(() => {
  ;(pElementRef.value as any).textContent = 'mounted!'

  // delay the text change after 2 seconds
  setTimeout(() => {
    delayedText.value = 'delayed text!'
  }, 2000)
})
</script>

<template>
  <h1>Lifecycle</h1>

  <p ref="pElementRef">hello</p>

  <p>Delayed text: {{ delayedText }}</p>
</template>
