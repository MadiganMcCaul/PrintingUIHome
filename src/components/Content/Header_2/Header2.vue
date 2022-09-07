<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="Header2-Container">
    <div class="Header2-Title-Container"></div>
  </div>
</template>

<style scoped>
.Header2-Container {
  box-sizing: border-box;
  height: 232px;
  min-width: 200vh;
  overflow: hidden;
  border: 1px solid #ffffff;
  background-color: #2b4a5e;
  top: 0;
  position: fixed;
  padding: 0;
  margin: 0;
  left: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 97;
}

/* .Header2-Title-Container{
    box-sizing: border-box;
    width: 400px;
    height: 63px;
    background-color: #C9282D;

    } */
</style>
