<template>
    <!-- v-bind:class o v-bind:style es la forma completa-->
    <p :class="{
        'danger': hasError,
        'success': !hasError
    }" :style="{
    backgroundColor: c
}">El mensaje se ha enviado satisfactoriamente.</p>

    <!-- v-on:click es la forma completa-->
<button @click="handleClick">Cambiar color</button>
</template>

<script lang="ts" setup>
import {ref} from 'vue'
let hasError = false;
let c = ref('#ccc');

const handleClick = () => c.value = '#1d1d1d';

</script>

<style>
.danger {
    color: red;
}

.success {
    color: greenyellow;
}
</style>