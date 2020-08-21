<template>
    <nav>
      <ul>
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/recipes">Recipes</nuxt-link></li>
        <li><nuxt-link to="/about">About</nuxt-link></li>
      </ul>
    </nav>
</template>

<script>
export default {
name: "header"
}
</script>

<style scoped>
nav {
  width: 100%;
  height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #0d0d1d;
}

ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

li {
  margin: 0 10px;
}
a{
  list-style-type: none;
  text-decoration: none;
  color: white;
}
</style>
