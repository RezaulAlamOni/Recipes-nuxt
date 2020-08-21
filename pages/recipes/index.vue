<template>
  <section class="recipes">

    <Recipes
      thumbnil="https://i1.wp.com/www.eatthis.com/wp-content/uploads/2019/10/pumpkin-pad-thai-recipe.jpg?resize=640%2C360&ssl=1"
      title="Sea Food Salad"
      preview-text="More tested"
    />
    <Recipes
      thumbnil="https://food.fnr.sndimg.com/content/dam/images/food/fullset/2017/12/10/0/WU1712H_Cauliflower-Mac-and-Cheese_s4x3.jpg.rend.hgtvcom.616.462.suffix/1580140849133.jpeg"
      title="Sea Food Salad 2"
      preview-text="More tested Goog newvcasr"
    />
  </section>

</template>

<script>
import Recipes from "../../components/Recipes";
export default {
  name: "index.vue",
  components: {Recipes},
  comments : {
    Recipes
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
