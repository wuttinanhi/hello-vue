<script setup lang="ts">
import ConditionalRendering from '@/components/ConditionalRendering.vue'
import CounterComp from '@/components/CounterComp.vue'
import InputExample from '@/components/InputExample.vue'
import TodoList from '@/components/TodoList.vue'
import LifeCycle from '@/components/LifeCycle.vue'
</script>

<template>
  <h1>Basic Counter</h1>
  <CounterComp />
  <hr />

  <h1>Input Example</h1>
  <InputExample />
  <hr />

  <h1>Conditional Rendering</h1>
  <ConditionalRendering />
  <hr />

  <h1>Todo List</h1>
  <TodoList />
  <hr />

  <h1>Lifecycle</h1>
  <LifeCycle />
  <hr />
</template>
