<script setup lang="ts">
const { count, increment, decrement, reset } = useCounter();
</script>

<template>
  <div>
    <button @click="increment">Incrementar</button>
    <button @click="decrement">Decrememntar</button>
    <button @click="reset">Reiniciar</button>
    <p>valor: {{ count }}</p>
  </div>
</template>
