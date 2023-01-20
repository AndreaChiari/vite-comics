<script>

import AppHeader from './components/AppHeader.vue'
import Main from './components/main.vue'
import Footer from './components/footer.vue'

export default {
  name: 'vite comics',
  components: {
    AppHeader, Main, Footer
  }
}
</script>

<template>
  <div class="main-container">
    <AppHeader></AppHeader>
    <main></main>
    <footer></footer>
  </div>
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