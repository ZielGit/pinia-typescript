<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
import { useCounterStore } from '@/stores/counter'

const counterStore = useCounterStore();

</script>

<template>
  <main>
    <TheWelcome />
    <h1>Home View: {{ counterStore.count }}</h1>
    <h3>Números de cambios: {{ counterStore.numberOfChanges }}</h3>
  </main>
</template>
