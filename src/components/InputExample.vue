<script setup lang="ts">
import { ref } from 'vue'

const myText = ref('')

function onInput(event: Event) {
  myText.value = (event.target as HTMLInputElement)?.value
}
</script>

<template>
  <h1>Input Example</h1>
  <input type="text" :value="myText" @input="onInput" />
  <p>{{ myText }}</p>
</template>
