<script lang="ts" setup>
const count = ref(0);
const countPorDos = computed(() => count.value * 2);

const incrementar = () => (count.value += 1);
const decrementar = () => (count.value -= 1);
</script>

<template>
  <div>
    <h1>Counter 2</h1>
    <p>{{ countPorDos }}</p>

    <button @click="incrementar">incrementar</button>
    <button @click="decrementar">incrementar</button>
  </div>
</template>
