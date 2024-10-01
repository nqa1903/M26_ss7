<template>
    <div>
        <ProductChild :id="products.id" :name="products.name" :price="products.price" :quantity="products.quantity"></ProductChild>
    </div>
</template>

<script setup>
    import ProductChild from './ProductChild.vue'
    const products = {
        id : 1,
        name : "Bưởi ba rọi",
        price : 12000,
        quantity : 10,
    }
</script>

<style scoped>

</style>