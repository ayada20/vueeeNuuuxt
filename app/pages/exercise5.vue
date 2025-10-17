<script lang="ts" setup>
const count = ref(0);

const incrementar = () => count.value++;
const decrementar = () => count.value--;
</script>

<template>
  <h1>{{ count }}</h1>
  <button @click="incrementar" v-show="!(count === 10)">incrementar</button>
  <button @click="decrementar" v-show="!(count === 0)">decrementar</button>
</template>

<style></style>
