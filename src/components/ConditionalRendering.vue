<script setup lang="ts">
import { ref } from 'vue'

const shouldShow = ref(true)
function toggle() {
  shouldShow.value = !shouldShow.value
}
</script>

<template>
  <button @click="toggle">Toggle Show</button>

  <div v-if="shouldShow">
    <p>Should show ✅</p>
  </div>

  <div v-else>
    <p>Should not show ❌</p>
  </div>
</template>
