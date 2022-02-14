<template>
  <Header />
  <div class="app-container">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <!-- <router-link to="/about">About</router-link> -->
    </div>
    <router-view />
  </div>
</template>

<script setup lang="ts">
import { Header } from "./components";
</script>
<style lang="scss">
@import "./styles/index.scss";
.app-container {
  margin: 0 32px;
}
#nav {
  display: none;
}
</style>
