<template>
    <div>
      ----- TodoApp Component -----
      <p>Id to delete: {{ idToDelete }}</p>
      <TodoItem @delete-item="handleDelete" />
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  import TodoItem from './TodoItem.vue';
  
  const idToDelete = ref(""); 
  
  // Hàm xử lý khi nhận sự kiện từ component con
  const handleDelete = () => {
    idToDelete.value++; 
  };
  </script>
  
  <style scoped>
  </style>
  