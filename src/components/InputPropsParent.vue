<script setup lang="ts">
import { ref } from 'vue'
import InputPropsChild from './InputPropsChild.vue'

const greeting = ref('Hello from parent')

function changeGreeting() {
  greeting.value = 'Hello from parent, updated!'
}
</script>

<template>
  <h1>Input Props</h1>

  <InputPropsChild :msg="greeting" />

  <button @click="changeGreeting">Change greeting</button>
</template>
