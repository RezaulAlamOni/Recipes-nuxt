<template>
  <article class="recipe">
    <div class="thumbnill"
         :style="{backgroundImage: 'url('+thumbnil+')'}"></div>
    <div>{{ title }}</div>
    <p>{{ previewText }}</p>
  </article>
</template>

<script>
export default {
  name: "Recipes",
  props: ['thumbnil', 'title', 'previewText']
}
</script>

<style scoped>
.recipe {
  box-sizing: border-box;
  width: 280px;
  padding: 8px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #aaa;
  margin: 10px;
}

.thumbnill {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 200px;
}
</style>
