<template>
    <ul>
        <!-- <li  v-for="(country, index) in countries" :key="index">{{ country.name }}</li> --> <!-- Es necesario pasarle una :key para que itere correctamente, me gusta mas ponerle un index -->
        <li  v-for="country in countries" :key="country.code">{{ country.name }}</li>
    </ul>
</template>


<script lang="ts" setup>
import {Ref, ref} from 'vue';

interface IDcountry {
    code: string,
    name: string
}

let countries:Ref<Array<IDcountry>> = ref([
    {
        code: 'es',
        name: 'Spain'
    },
    {
        code: 'en',
        name: 'UK'
    },
    {
        code: 'fr',
        name: 'France'
    },
    {
        code: 'it',
        name: 'Italy'
    },
    {
        code: 'pt',
        name: 'Portugal'
    },
])

</script>

<style scoped>
</style>