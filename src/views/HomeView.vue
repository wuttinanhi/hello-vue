<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <!-- <main>
    <TheWelcome />
  </main> -->

  <h1>COUNT: {{ count }}</h1>

  <button @click="increment">Increment</button>
</template>
