<template>
  <div id="app">
    <homepage></homepage>
  </div>
</template>

<script>
import Homepage from "./components/homepage.vue";

export default {
  name: "App",
  components: {
    Homepage,
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&family=Oswald&family=Raleway:wght@400;500;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Sansita+Swashed:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500;600;700&family=Sansita+Swashed:wght@500&display=swap');

#app {
  font-family: 'Raleway', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html,
body {
  padding: 0;
}

body {
  margin: 0 2rem 0 2rem;
}
</style>
