<!-- Button.vue -->
<template>
    <div>
      <input type="text" v-model="name" placeholder="Masukkan nama">
      <button @click="emitData">Click Me!</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: ''
      };
    },
    methods: {
      emitData() {
        const data = {
          name: this.name,
        };
        this.$emit('buttonClicked', data);
      }
    }
  }
  </script>
  <style>
  .button-container {
    text-align: center;
  }
  .input-field {
    padding: 8px;
    margin-right: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
  }
  .btn {
    padding: 8px 16px;
    background-color: #007bff;
    color: #ff2e9a;
    border: none;
    border-radius: 3px;
    cursor: pointer;
  }
  .btn:hover {
    background-color: #0056b3;
  }
  </style>