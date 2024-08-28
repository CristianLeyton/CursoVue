<template>
    <form action="">
        <input type="text" v-model="inputText"> <!-- Vincula este input con una variable en el script -->
        <input type="checkbox" name="" id="" v-model="agree"> Acepto los terminos y condiciones
        <select name="" id="" v-model="country">
            <option value="Spain">Spain</option>
            <option value="Uk">UK</option>
            <option value="France">France</option>
        </select>

    </form>

    <h1>{{ inputText }}</h1>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';
    let inputText = ref(''); //Vinculo esta variable con el input en el script
    let agree = ref(true);
    let country = ref('France')
</script>

<style scoped>
</style>