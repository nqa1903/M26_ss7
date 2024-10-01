<template>
    <div>
        ----- Parent Company -----
        <p>Parent Compant : {{ company }}</p>
        <ChildrenComponent :company="company"></ChildrenComponent>
    </div>
</template>

<script setup>
    import ChildrenComponent from './ChildrenComponent.vue';
    import {ref} from "vue";
    const company = ref("Rikkei Academy")
</script>

<style scoped>

</style>