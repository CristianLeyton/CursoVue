<template>
<!--     <h1 v-if="age < 18">Eres menor de Edad</h1>
    <h2 v-else>Eres mayor de Edad</h2> -->
    <h1 v-show="age < 18">Eres menor de Edad</h1> <!-- v-show carga el elemento en el DOM con un display-none si no se cumple la condicion -->
    <h2 v-show="age >= 18">Eres mayor de Edad</h2>
</template>

<script lang="ts" setup>

    let age = 18;

</script>

<style scoped>
</style>