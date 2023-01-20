<script>

import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import Footer from './components/footer.vue'

export default {
  name: 'vite comics',
  components: {
    AppHeader, AppMain, Footer
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <footer></footer>
</template>

<style>
/* Generics */
* {
  font-family: 'Open Sans', sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
  height: auto;
}

.main-container {
  width: 1200px;
  height: 100vh;
  margin: auto;
}
</style>