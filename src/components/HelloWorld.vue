<template>
  <h1>{{ name }}</h1>
  <!-- recorrer objeto -->
  <ul>
      <li v-for="(value, propiedad) in objetoFruta" :key="value">
          {{ propiedad }} : {{ value }}
      </li>
  </ul>
</template>

<script setup>
const name = 'Vite + Vue';
const objetoFruta = {
  id: '1',
  name: 'piña',
  precio: '2.000',
  descripcion: 'pina amarilla',
};
</script>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
