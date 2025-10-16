<script setup lang="ts">
const { count, increment, decrement, reset } = useCounter();
</script>

<template>
  <div>
    <p>
      {{ count }}
    </p>

    <button @click="increment" :style="{ color: count >= 10 ? 'green' : '' }">
      Incrementar
    </button>
  </div>
</template>
