<template>
    <div>
        ----- Children Company -----
        <p>Children Company : {{ props.company }}</p>
    </div>
</template>

<script setup>
    const props = defineProps(["company"])
</script>

<style scoped>

</style>