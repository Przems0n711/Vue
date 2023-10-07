<template>
  <div id="app">
    <h1>{{ message }}</h1>
    <button @click="changeMessage">Change Message</button>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const message = ref('Hello, Vue with TSX!');

const changeMessage = () => {
  message.value = 'Vue with TSX is awesome!';
};
</script>