<script lang="ts" setup>
const count = ref(0);
const incrementar = () => count.value++;
const decrementar = () => count.value--;
</script>

<template>
  <div>
    <h1><TheTitle /></h1>

    <h1>{{ count }}</h1>
    <button @click="incrementar">incrementar</button>
    <button @click="decrementar">decrementar</button>
  </div>
</template>

<style></style>
