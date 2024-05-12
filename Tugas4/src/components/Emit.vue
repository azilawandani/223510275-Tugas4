<!-- Emit.vue -->
<template>
    <div class="emit-container">
      <h2 style="text-align: center;">Emit Component</h2>
      <Button @buttonClicked="handleButtonClick" />
      <Slot :data="buttonData || {}" />
    </div>
  </template>
  
  <script>
  import Button from './Button.vue';
  import Slot from './Slot.vue';
  
  export default {
    components: {
      Button,
      Slot
    },
    data() {
      return {
        buttonData: {}
      };
    },
    methods: {
      handleButtonClick(data) {
        this.buttonData = data;
      }
    }
  }
  </script>
  
  <style>
  .emit-container {
    margin: 20px auto;
    padding: 20px;
    border: 1px solid palevioletred;
    border-radius: 5px;
    background-color: bisque;
  }
  </style>
  