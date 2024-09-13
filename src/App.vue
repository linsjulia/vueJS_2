<template>
  <NavPage></NavPage>
  <ContentPage></ContentPage>
  <FooterPage></FooterPage>
</template>

<script>
import NavPage from './components/default/NavPage.vue';
import ContentPage from './components/default/ContentPage.vue';
import FooterPage from './components/default/FooterPage.vue';

export default {
  name: 'App',
  component: {
    NavPage, ContentPage, FooterPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
