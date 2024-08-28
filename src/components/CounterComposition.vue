<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts" setup> //el atributo "setup" hace todo lo que esta comentado aqui abajo: 
import { /* defineComponent, */ ref } from 'vue';
/* export default defineComponent({
    name: 'CounterComposition',
    setup() { */
    let counter = ref(0); //debo importar y usar la funcion ref() para inidicar que quiero interactividad en esta variable
    const addCounter = () => {
        counter.value++; //ref devuelve un objeto asi que necesito acceder a el por su atributo .value
    }
/*     return {counter, addCounter}
    }
}) */

</script>

<style scope></style>