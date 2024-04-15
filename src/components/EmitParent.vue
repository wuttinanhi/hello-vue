<script setup lang="ts">
import { ref } from 'vue'
import EmitChild from './EmitChild.vue'

const childMsg = ref('No child msg yet')
</script>

<template>
  <h1>Emit</h1>

  <EmitChild @myresponse="(msg) => (childMsg = msg)" />
  <p>Message from child: {{ childMsg }}</p>
</template>
