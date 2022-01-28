<template>
  <div id="app">
    <Header/>
    <Main />
    <footer>
      <FooterTop />
      <FooterMiddle />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import FooterTop from './components/FooterTop.vue'
import FooterMiddle from './components/FooterMiddle.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    FooterTop,
    FooterMiddle,
    FooterBottom
  }
}
</script>

<style lang="scss">
@import "./assets/style/global.scss";
@import "./assets/style/partials/variables.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
