<template>
  <section>
    <div v-for="(item, i) in footerTopItems" :key="i" class="footer-top-item">
      <a :href="item.url"><img :src="require('../assets/img/' + item.img)" alt=""></a>
      <div class="footer-top-item-name">{{item.text}}</div>
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
          url: "#",
          img: "buy-comics-digital-comics.png"
        },
        {
          text: "DC Merchandise",
          url: "#",
          img: "buy-comics-merchandise.png"
        },
        {
          text: "Subscription",
          url: "#",
          img: "buy-comics-subscriptions.png"
        },
        {
          text: "Comic Shop Location",
          url: "#",
          img: "buy-comics-shop-locator.png"
        },
        {
          text: "DC Power Visa",
          url: "#",
          img: "buy-dc-power-visa.svg"
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/style/global.scss";
@import "../assets/style/partials/variables.scss";

section {
  background-color: $mainColor;
}
</style>