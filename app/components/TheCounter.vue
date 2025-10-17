<script lang="ts" setup>
const count = ref(0);
const countPorDos = computed(() => count.value * 2);

const incrementar = () => (count.value += 1);
const decrementar = () => (count.value -= 1);

const message = ref("m");
watch(count, (valorNuevo) => {
  if (valorNuevo === 0) {
    message.value = "estas en el valor minimo;";
  } else if (valorNuevo === 10) {
    message.value = "estas en el valor maximo";
  } else if (valorNuevo >= 0 && valorNuevo <= 10) {
    message.value = "estas en los parametros adecuados";
  } else {
    message.value = "";
  }
});
</script>

<template>
  <div>
    <h1>Counter 3 watchers</h1>
    <p>{{ count }}</p>

    <button @click="incrementar">incrementar</button>
    <button @click="decrementar">decrementar</button>
    <p>{{ message }}</p>
  </div>
</template>
