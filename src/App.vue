<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  name: 'Dc comics',
  components: { AppHeader, AppMain, AppFooter }
}
</script>

<template>

  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>

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

header {
  font-family: "Open Sans", sans-serif;
}

main,
footer {
  font-family: "Open Sans Condensed", sans-serif;
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
