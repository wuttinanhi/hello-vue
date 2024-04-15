<script setup>
import { ref, onMounted } from 'vue'

const pElementRef = ref(null)
const delayedText = ref('')
onMounted(() => {
  pElementRef.value.textContent = 'mounted!'

  // delay the text change after 2 seconds
  setTimeout(() => {
    delayedText.value = 'delayed text!'
  }, 2000)
})
</script>

<template>
  <p ref="pElementRef">hello</p>

  <p>Delayed text: {{ delayedText }}</p>
</template>
