<!-- App.vue -->
<template>
  <div id="app">
    <h1>Universitas Islam Riau</h1>
    <Emit />
  </div>
</template>

<script>
import Emit from './components/Emit.vue';

export default {
  name: 'App',
  components: {
    Emit
  }
}
</script>

<style>
#app {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid palevioletred;
  border-radius: 5px;
  background-color: pink;
}
</style>
