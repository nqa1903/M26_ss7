<template>
  <div>
    Câu 1
    <ParentComponent></ParentComponent>
  </div>
  <div>
    Câu 2
    <ProductParent></ProductParent>
  </div>
  <div>
    Câu 3
    <CountParent></CountParent>
  </div>
  <div>
    Câu 4
    <TodoApp></TodoApp>  
  </div>
  <div>
    Câu 5
    <Modal>
      <template #header>
        <h3>Thông báo từ hệ thống</h3>
      </template>
      <template #content>
        <p>Đây là nội dung của modal . Bạn có thể đóng modal bằng cách nhấn vào nút close</p>
      </template>
      <template #footer>
        <button>Close</button>
      </template>
    </Modal>
  </div>
  <div>
    Câu 6
    <Card>
      <template #header>
        Thông tin sản phẩm
      </template>
      <template #body>
        Đây là mô tả ngắn gọn về sản phẩm này. Sản phẩm có các tính năng nổi bật và giá cả hợp lý.
      </template>
      <template #footer>
        <button @click="viewDetails">Xem chi tiết</button>
      </template>
    </Card>
  </div>
</template>

<script setup>
  import ParentComponent from "./components/ParentComponent.vue"
  import ProductParent from "./components/ProductParent.vue"
  import CountParent from "./components/CountParent.vue"
  import TodoApp from "./components/TodoApp.vue";
  import Modal from "./components/Modal.vue";
  import Card from "./components/Card.vue";
  
</script>
  
<style scoped>

</style>