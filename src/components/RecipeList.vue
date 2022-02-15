<template>
  <div class="container">
    <div class="container-item">
      <RecipeItem></RecipeItem>
    </div>
  </div>
</template>

<script setup lang="ts">
import RecipeItem from "./RecipeItem.vue";
</script>

<style scoped lang="scss">
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 0.75vh;
  border: 1px black solid;
}
</style>
