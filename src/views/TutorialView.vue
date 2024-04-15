<script setup lang="ts">
import ConditionalRendering from '@/components/ConditionalRendering.vue'
import CounterComp from '@/components/CounterComp.vue'
import EmitParent from '@/components/EmitParent.vue'
import InputExample from '@/components/InputExample.vue'
import InputPropsParent from '@/components/InputPropsParent.vue'
import LifeCycle from '@/components/LifeCycle.vue'
import SlotParent from '@/components/SlotParent.vue'
import TodoList from '@/components/TodoList.vue'
import Watcher from '@/components/Watcher.vue'
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

  <h1>Watcher</h1>
  <Watcher />
  <hr />

  <h1>Input Props</h1>
  <InputPropsParent />
  <hr />

  <h1>Emit</h1>
  <EmitParent />
  <hr />

  <h1>Slot</h1>
  <SlotParent />
  <hr />
</template>
