<template>
  <section class="recipes">
    <article class="recipe">
      <div class="thumbnill" style="background-image: url('https://i1.wp.com/www.eatthis.com/wp-content/uploads/2019/10/pumpkin-pad-thai-recipe.jpg?resize=640%2C360&ssl=1')"></div>
      <div>Title</div>
      <p>Some nice text</p>
    </article>
    <article class="recipe">
      <div class="thumbnill" style="background-image: url('https://food.fnr.sndimg.com/content/dam/images/food/fullset/2017/12/10/0/WU1712H_Cauliflower-Mac-and-Cheese_s4x3.jpg.rend.hgtvcom.616.462.suffix/1580140849133.jpeg')"></div>
      <div>Title</div>
      <p>Some nice text</p>
    </article>
  </section>

</template>

<script>
export default {
name: "index.vue"
}
</script>

<style scoped>
.recipes {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}
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
