<script setup>
import { RouterView } from 'vue-router';

</script>

<template>
  <div class="layout d-flex justify-content-center">
    <div class="container">
      <RouterView></RouterView>
    </div>
  </div>
</template>

<style scoped>
  .layout {
    min-height: 100vh;
    background: linear-gradient(
      70deg,
      #0f0f0f,
      #383838
    );
  }

</style>
