<template>
    <div class="container">
        <slot name="header" class="pd"></slot>
        <hr>
        <slot name="content" class="pd"></slot>
        <hr>
        <slot name="footer" class="pd ps"></slot>
    </div>
</template>

<script setup>

</script>

<style scoped>
    .container {
        width: 320px;
        border: 1px solid black;
    }
    .pd{
        padding: 4px;
    }
</style>