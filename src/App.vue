<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
  name: 'Dc comics',
  components: { AppHeader, AppMain }
}
</script>

<template>

  <app-header></app-header>
  <app-main></app-main>
  <footer></footer>

</template>

<style>
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generics */
body {
  min-height: 100vh;
}

img {
  max-width: 100%;
  height: auto;
  display: block;
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
}


/* Utils */
.container {
  margin: 0 auto;
  max-width: 1000px;
}
</style>
