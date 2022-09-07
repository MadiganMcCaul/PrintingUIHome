<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header/Header.vue";
import Sidebar from "./components/Sidebar/Sidebar.vue";
import Content from "./components/Content/Content.vue";
</script>

<template>
  <div class="Page">
    <Header />
    <div class="Sidebar_Content">
      <Sidebar />
      <Content />
    </div>
  </div>
</template>

<style scoped>

.Page {
  box-sizing: border-box;
  height: 1024px;
  width: 1920px;
  display: flex;
  flex-direction: column;
}

.Sidebar_Content {
  display: flex;
  height: 908px;
  width: 1920px;
  flex-direction: row;
}
</style>
