<template>
  <section>
    <div v-for="(item, i) in footerTopItems" :key="i" class="footer-top-item">
      <img :src="'../assets/img/' + item.img" alt="">
      <div class="footer-top-item-name"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FooterTop',
  data() {
    return {
      footerTopItems: [
        {
          text: "Digital Comics",
          img: "buy-comics-digital-comics.png"
        },
        {
          text: "DC Merchandise",
          img: "buy-comics-merchandise.png"
        },
        {
          text: "Subscription",
          img: "buy-comics-subscriptions.png"
        },
        {
          text: "Comic Shop Location",
          img: "buy-comics-shop-locator.png"
        },
        {
          text: "DC Power Visa",
          img: "buy-dc-power-visa.svg"
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  background-color: #0282f9;
}
img {
  width: 100px;
  height: 100px;
}
</style>
