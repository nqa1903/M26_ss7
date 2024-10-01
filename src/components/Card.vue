<template>
    <div class="card">
      <div class="card-header">
        <slot name="header"></slot>
      </div>
      <div class="card-body">
        <slot name="body"></slot>
      </div>
      <div class="card-footer">
        <slot name="footer"></slot>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Card',
  }
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #ddd;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 16px;
  }
  
  .card-header {
    font-weight: bold;
    font-size: 1.2rem;
    margin-bottom: 12px;
  }
  
  .card-body {
    margin-bottom: 12px;
  }
  
  .card-footer {
    text-align: right;
  }
  </style>
  