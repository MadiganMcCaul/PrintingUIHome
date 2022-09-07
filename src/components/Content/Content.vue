<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Header2 from "./Header_2/Header2.vue";
</script>

<template>
  <div class="content-container">
    <Header2 />
  </div>
</template>

<style scoped>
    .content-container {
        display: flex;
        box-sizing: border-box;
        min-width: 1146px;
        min-height: 911px;
        position: fixed;
        justify-content: flex-end;
        align-self: flex-end;
        
    }
</style>