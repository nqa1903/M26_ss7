<template>
    <div>
        ----- Parent Component -----
        <p>count : {{ number }}</p>
        <CountChild @number="handleNumber" :numbers="number"></CountChild>
    </div>
</template>

<script setup>
    import CountChild from './CountChild.vue'
    import {ref} from "vue";
    const number = ref(0);
    const handleNumber = (updateNumber) =>{
        number.value = updateNumber;
    }
</script>

<style scoped>

</style>