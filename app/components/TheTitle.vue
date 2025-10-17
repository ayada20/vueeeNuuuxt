<script lang="ts" setup>
const props = defineProps({
  propTitle: String,
});
</script>

<template>
  <h1 class="title">
    {{ propTitle }}
  </h1>
  <h1>Contador</h1>
</template>
