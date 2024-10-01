<template>
  <div>
    ----- Child Component -----
    <p><button @click="handleIncrease">Increase</button></p>
  </div>
</template>

<script setup>
    const props = defineProps(["numbers"])
    const emit = defineEmits(["number"]);
    const handleIncrease = () =>{
        emit("number" , props.numbers + 1);
    }
</script>

<style scoped></style>
