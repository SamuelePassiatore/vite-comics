<script>
import AppHeader from './components/AppHeader.vue'
export default {
  name: 'Dc comics',
  components: { AppHeader }
}
</script>

<template>

  <app-header></app-header>
  <main></main>
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

a {
  text-decoration: none;
}

/* Utils */
.container {
  margin: 0 auto;
  max-width: 1000px;
}
</style>
