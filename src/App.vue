<script>

import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'vite comics',
  components: {
    AppHeader, AppMain, AppFooter,
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style>
/* Generics */
* {
  font-family: 'Open Sans', sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  width: 1200px;
  height: 100vh;
  margin: auto;
}
</style>