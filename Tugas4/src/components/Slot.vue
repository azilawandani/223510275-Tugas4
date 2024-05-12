<!-- Slot.vue -->
<template>
    <div class="slot-container">
      <h3>Data yang dimasukkan oleh pengguna: {{ data.name }}</h3>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      data: {
        type: Object,
        default: () => ({})
      }
    }
  }
  </script>
  
  <style>
  .slot-container {
    margin-top: 20px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #f0f0f0;
  }
  </style>
  