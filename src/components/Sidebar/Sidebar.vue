<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <Sider>
    <div class="nav-bar">
      <nav>
        <div class="container first">
          <RouterLink to="/"
            ><img src="@/assets/Logos/Home.svg" class="navbar-image icon"
          /></RouterLink>
          <h1 class="button-text">Home</h1>
        </div>
        <div class="container second">
          <RouterLink to="/"
            ><img src="@/assets/Logos/Order.svg" class="navbar-image icon"
          /> <img src="@/assets/Logos/Add.svg" alt="" class="nav-extras-add icon" /></RouterLink>
          <h1 class="button-text">Create Order</h1>
        </div>

        <div class="container third">
            <RouterLink to="/"
            ><img src="@/assets/Logos/Order.svg" class="navbar-image icon"
          /><img src="@/assets/Logos/History.svg" alt="" class="nav-extras-history icon" /></RouterLink>
          <h1 class="button-text">Order History</h1>
        </div>

        <div class="container fourth">
            <RouterLink to="/"
            ><img src="@/assets/Logos/Product.svg" class="navbar-image icon"/></RouterLink>
          <h1 class="button-text">Products</h1>
        </div>

        <div class="container fifth">
            <RouterLink to="/"
            ><img src="@/assets/Logos/Printer.svg" class="navbar-image icon"/></RouterLink>
          <h1 class="button-text">Printers</h1>
        </div>

        <div class="container sixth">
            <RouterLink to="/"
            ><img src="@/assets/Logos/Filament.svg" class="navbar-image icon"/></RouterLink>
          <h1 class="button-text">Filaments</h1>
        </div>
      </nav>
    </div>
  </Sider>
  <router-view />
</template>

<style scoped>
Sider {
  box-sizing: border-box;
  min-width: 294px;
  height: 100%;
  /* margin-top: 115px; */

  background: #2b4a5e;

  display: flex;
  flex-direction: column;
  overflow: hidden;

  border: 1px solid #ffffff;
  background-color: #2b4a5e;

  transition: 0.3s ease;

  top: 0;
  /* position: fixed; */
  left: 0;
  z-index: 99;
}

nav {
  flex-direction: column;
  text-align: left;
  display: flex;
  place-items: right;
  padding-left: 0px;
  padding-top: 26px;
  gap: 26px;
  /* width: 120px; */
}

.container {
  display: flex;
  justify-content: space-evenly;
  text-align: center;
  align-content: center;
  align-items: center;
  width: 100%;
  padding-right: 2rem;
}

.first > h1 {
  color: red;
}

.second {
}
.container > h1 {
  color: white;
}

.icon {
    filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(90deg) brightness(104%) contrast(104%);
}

.navbar-image {
  width: 3rem;
  height: 3rem;
  /*filter: invert(45%) sepia(40%) saturate(5837%) hue-rotate(339deg) brightness(94%) contrast(92%);*/
  /* filter: invert(19%) sepia(49%) saturate(5995%) hue-rotate(348deg) brightness(84%) contrast(85%); */
}

.navbar-image:hover {
    filter: invert(19%) sepia(49%) saturate(5995%) hue-rotate(348deg) brightness(84%) contrast(85%);
}

.nav-extras-history:hover {
    filter: invert(19%) sepia(49%) saturate(5995%) hue-rotate(348deg) brightness(84%) contrast(85%);
}

.nav-extras-add:hover {
    filter: invert(19%) sepia(49%) saturate(5995%) hue-rotate(348deg) brightness(84%) contrast(85%);
}

.nav-extras-history {
    margin-bottom: 6px;
    margin-left: 7px;
}

.nav-extras-add {
    margin-bottom: 6px;

}



img {
  margin-top: px;
}
</style>
