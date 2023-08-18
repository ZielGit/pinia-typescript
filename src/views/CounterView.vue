<template>
    <div>
        <h1>Counter View: {{ counterStore.count }}</h1>
        <button @click="counterStore.increment()">+1</button>
    </div>
</template>

<script lang="ts" setup>
import { useCounterStore } from '@/stores/counter';

const counterStore = useCounterStore();
</script>
