// composables/useCounter.ts import { ref } from "vue"; export function
useCounter() { const count = ref(0); function increment() { count.value++; } }
-No es necesario el import y la funcion no devuelve nada.

<script setup lang="ts">
const items = ref(["Apple", "Banana", "Cherry"]);
</script>
<template>
  <ul>
    <li v-for="(item, index) in items" :key="index">
      {{ item }}
    </li>
  </ul>
  <!-- import no es necesario ya que usa el setup, al script le falta lang="ts", en vez de usar key="index 
  mejor llamarlo de otra forma como id y que sea el conjunto de dos paramentros como el nombre y la edad, 
  los tipos no tienen tipo -->
</template>

<script lang="ts" setup>
const counter = ref(0);
</script>
<template>
  <p v-if="counter === 10">Número, {{ counter }}</p>
  <!-- al script le falta el setup y el lang="ts", siempre debe haber un div dentro del template 
    y meter dentro del div el codigo falta un igual ya que hay que usar 3 iguales obligatoriamente,
     para que counter pueda ser leido debe meterse el ref-->
</template>
