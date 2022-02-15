<template>
  <div v-for="recipeItem in recipeItems" :key="recipeItem">
    <div>
      <div class="item-photo">
        <img :src="recipeItem.photo" />
      </div>
      <div>{{ recipeItem.name }}</div>
      <div>{{ recipeItem.description }}</div>
      <ul v-for="ingredient in recipeItem.ingredient" :key="ingredient">
        <li>{{ ingredient }}</li>
      </ul>
    </div>
  </div>
</template>

<script setup lang="ts">
const recipeItems = [
  {
    name: "Салат 1",
    description: "Очень вкусный салат",
    photo: "https://attuale.ru/wp-content/uploads/2018/11/129_image.jpg",
    ingredient: ["Картошка", "Сыр", "Хлеб"],
  },
  {
    name: "Салат 2",
    description: "Очень вкусный салат",
    photo: "https://attuale.ru/wp-content/uploads/2018/11/129_image.jpg",
    ingredient: ["Картошка", "Сыр", "Хлеб"],
  },
  {
    name: "Салат 3",
    description: "Очень вкусный салат",
    photo: "https://attuale.ru/wp-content/uploads/2018/11/129_image.jpg",
    ingredient: ["Картошка", "Сыр", "Хлеб"],
  },
];
</script>

<style scoped lang="scss">
.item-photo {
  width: 100px;
  height: 100px;
  img {
    width: 100%;
    height: 100%;
  }
}
</style>
