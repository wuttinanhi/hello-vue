<script setup lang="ts">
import { reactive } from 'vue'

const counter = reactive({
  count: 0,
  increment() {
    counter.count++
  }
})
</script>

<template>
  <h1>Basic Counter</h1>

  <h1>COUNT: {{ counter.count }}</h1>

  <button @click="counter.increment">Increment</button>
</template>
