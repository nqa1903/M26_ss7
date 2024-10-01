<template>
    <div>
        Dữ liệu trong component con : 
        <ul>
            <li>Id : {{ props.id }}</li>
            <li>Product Name : {{ props.name }}</li>
            <li>Price : {{ props.price }}đ</li>
            <li>Quantity : {{ props.quantity }}</li>
        </ul>
    </div>
</template>

<script setup>
    const props = defineProps(["id" , "name" , "price" , "quantity"]);
</script>

<style scoped>

</style>