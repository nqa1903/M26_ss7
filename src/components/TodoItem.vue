<template>
    <div>
      ----- TodoItem Component -----
      <p><button @click="handleDelete">Delete</button></p>
    </div>
  </template>
  
  <script setup>
  import { defineEmits } from 'vue';
  
  // Phát sự kiện lên component cha
  const emit = defineEmits(['delete-item']);
  const handleDelete = () => {
    emit('delete-item'); 
  };
  </script>
  
  <style scoped>
  </style>
  