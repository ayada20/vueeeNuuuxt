<script setup lang="ts">
const emit = defineEmits<{
  (e: "sayHello", message: string): void;
}>();

function sendHello() {
  emit("sayHello", "holaaa");
}
</script>

<template>
  <div>
    <button @click="sendHello">Enviar saludo al padre</button>
  </div>
</template>
