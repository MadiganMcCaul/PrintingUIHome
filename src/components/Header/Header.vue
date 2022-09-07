<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="header-container">
    <div class="logo-container">
      <img
        alt="Sage logo"
        class="logo"
        src="@/assets/Logos/Sage_Logo.png"
        width="266"
        height="60"
      />
    </div>

    <div class="search-container">
      <nav2>
        <div class ="search-logo-holder">
          <img src="@/assets/Logos/Search Bar.svg" />
        </div>
        <div class="search-bar">
          <h1>Search here...</h1>
        </div>
      </nav2>
    </div>

    <div class="nav-container">
      <nav>
        <RouterLink to="/"><img src="@/assets/Logos/Settings.svg" class="icon"/></RouterLink>
        <RouterLink to="/"><img src="@/assets/Logos/Help.svg" class="icon"/></RouterLink>
        <RouterLink to="/"><img src="@/assets/Logos/Profile.svg" class="icon"/></RouterLink>
      </nav>
    </div>
  </div>
  <router-view />
</template>

<style scoped>
.header-container {
  box-sizing: border-box;
  height: 116px;

  min-width: 1920px;
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
  z-index: 98;
}

.nav-container {
  width: 30%;
}

.search-container {
  box-sizing: border-box;
  height: 116px;
  width: 633px;
  display: flex;
  align-items: center;
}

.icon {
  filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(90deg) brightness(104%) contrast(104%);
}

.icon:hover {
  filter: invert(19%) sepia(49%) saturate(5995%) hue-rotate(348deg) brightness(84%) contrast(85%);
}

.logo-container {
  box-sizing: border-box;
  height: 116px;
  width: 633px;

  background: #2b4a5e;
  display: flex;
  align-items: center;

  padding-left: 1rem;
}

nav {
  width: 70%;
  display: flex;
  justify-content: flex-end;
  gap: 2rem;
  text-align: right;
  margin-left: 1rem;
  /* margin-right: 5rem; */
}

img {
  /* margin-top: 26px; */
}

nav2 {
  box-sizing: border-box;
  padding-top: 0px;
  flex-direction: row;
  display: flex;
  align-items: center;

}

.search-logo-holder {
  box-sizing: border-box;
  height: 38px;
  width: 38px;
  display: flex;
  align-items: center;
  padding-left: 6px;

  background-color: #ffffff;
  border: 1px solid #000000;
  border-radius: 10px 0px 0px 10px;
}

.search-bar {
  box-sizing: border-box;
  height: 38px;
  width: 597px;

  background-color: #ffffff;
  border: 1px solid #000000;
  border-radius: 0px 10px 10px 0px;
  text-align: left;
  padding-left: 6px;
  align-content: center;
  font-size: 12px;
}
</style>
