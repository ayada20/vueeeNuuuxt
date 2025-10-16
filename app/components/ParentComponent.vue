<script setup lang="ts">
provide("message", "hola desde el componente padre al hijo");
</script>

<template>
  <div><ChildComponent /></div>
</template>
