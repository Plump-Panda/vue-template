<template>
  <MainPage msg="Welcome to Your Vue.js App"/>
</template>

<script>
import MainPage from './components/MainPage.vue'

export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>
#app {
  background-image: url('./assets/background.jpg');
  width: 100%;
  height: 100%;
}
</style>
