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
import Header from './components/macro/Header.vue'
import Main from './components/macro/Main.vue'
import FooterTop from './components/macro/FooterTop.vue'
import FooterMiddle from './components/macro/FooterMiddle.vue'
import FooterBottom from './components/macro/FooterBottom.vue'

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
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>