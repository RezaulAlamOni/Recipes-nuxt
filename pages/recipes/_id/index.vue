<template>


  <section class="single-recipes">
    <h1>{{ recipe.title }}</h1><br>
    <div>
      <img :src="recipe.thumbnil" alt="">
      <p>
        {{ recipe.previewText}}
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "index",
  asyncData(context) {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          recipe: [
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
          ].find(el => el.id === context.params.id)
        })
      }, 1500)
    })
  }
}
</script>

<style scoped>
.single-recipes {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
    flex-flow: column;
  padding: 30px;
}

</style>
