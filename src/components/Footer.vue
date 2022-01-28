<template>
  <footer>
    <FooterTop />
    <FooterMiddle />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from './footer-components/FooterTop.vue'
import FooterMiddle from './footer-components/FooterMiddle.vue'
import FooterBottom from './footer-components/FooterBottom.vue'

export default {
  name: 'Footer',
  components: {
    FooterTop,
    FooterMiddle,
    FooterBottom
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
