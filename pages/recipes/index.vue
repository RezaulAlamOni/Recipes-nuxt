<template>
  <section class="recipes">

    <Recipes v-for="recipe in recipes"
             :key="recipe.id"
             :thumbnil="recipe.thumbnil"
             :title="recipe.title"
             :preview-text="recipe.previewText"
             :id="recipe.id"
    />
  </section>

</template>

<script>
import Recipes from "../../components/Recipes";

export default {
  name: "index.vue",
  components: {Recipes},
  comments: {
    Recipes
  },
  asyncData() {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipes: [
            {
              id: "1",
              title: "DUEoD DISN",
              previewText: "DUEoD Pixxxaaz",
              thumbnil: "https://i1.wp.com/www.eatthis.com/wp-content/uploads/2019/10/pumpkin-pad-thai-recipe.jpg?resize=640%2C360&ssl=1",
            },
            {
              id: "2",
              title: "DFD DISN",
              previewText: "DU SD D aaz",
              thumbnil: "https://food.fnr.sndimg.com/content/dam/images/food/fullset/2017/12/10/0/WU1712H_Cauliflower-Mac-and-Cheese_s4x3.jpg.rend.hgtvcom.616.462.suffix/1580140849133.jpeg",
            }
          ]
        })
      }, 1500)
    })
  }

}
</script>

<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}


</style>
