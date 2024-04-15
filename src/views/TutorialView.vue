<script setup lang="ts">
import ConditionalRendering from '@/components/ConditionalRendering.vue'
import BasicCounter from '@/components/BasicCounter.vue'
import EmitParent from '@/components/EmitParent.vue'
import InputExample from '@/components/InputExample.vue'
import InputPropsParent from '@/components/InputPropsParent.vue'
import LifeCycle from '@/components/LifeCycle.vue'
import SlotParent from '@/components/SlotParent.vue'
import TodoList from '@/components/TodoList.vue'
import MyWatcher from '@/components/MyWatcher.vue'
import { ref } from 'vue'

const tutorialMap: { [key: string]: any } = {
  'Basic Counter': BasicCounter,
  'Input Example': InputExample,
  'Conditional Rendering': ConditionalRendering,
  'Todo List': TodoList,
  'Input Props': InputPropsParent,
  'Life Cycle': LifeCycle,
  Watcher: MyWatcher,
  'Slot Parent': SlotParent,
  'Emit Parent': EmitParent
}

const showingTutorial = ref('Basic Counter')
</script>

<template>
  <h1>Tutorial Stuff</h1>

  <button v-for="(value, key) in tutorialMap" :key="key" @click="showingTutorial = key.toString()">
    {{ key }}
  </button>

  <hr />

  <component :is="tutorialMap[showingTutorial]" />
</template>
