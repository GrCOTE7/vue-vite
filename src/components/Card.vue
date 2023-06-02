<!-- Card.vue -->
<template>
  <div class="cardGc7">
    <div class="card-header">
      <slot name="title"></slot>
    </div>
    <div class="card-body">
      <slot>Default Content</slot>
    </div>
  </div>
</template>

<style>
.cardGc7 {
  background-color: #ffffff;
  border: 1px solid #cccccc;
  padding: 10px;
  margin: 10px 0;
  border-radius: 7px;
}

.card-header {
  font-weight: bold;
  margin-bottom: 5px;
}
</style>
