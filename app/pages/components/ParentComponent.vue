<script setup lang="ts">
import ChildComponent from "@/pages/components/ChildComponent.vue";

function recibeHello(message: string) {
  console.log("message recibed", message);
  alert(message);
}
</script>

<template>
  <div>
    <h2>Parent component</h2>
    <ChildComponent @sayHello="recibeHello" />
  </div>
</template>
