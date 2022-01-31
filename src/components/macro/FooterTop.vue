<template>
  <section>
    <div class="container">
      <div v-for="(item, i) in footerTopItems" :key="i" class="footer-top-item">
        <a :href="item.url">
          <img :src="require('../../assets/img/' + item.img)" alt="">
          <span class="footer-top-item-name">{{item.text}}</span>
        </a>
      </div>
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
@import "../../assets/style/global.scss";
@import "../../assets/style/partials/variables.scss";

section {
    background-color: $mainColor;
}

.container {
  height: 150px;

  font-family: 'Bangers', cursive;
  font-size: 14px;

  display: flex;
  justify-content: space-around;
}

.footer-top-item {
  width: 236px;
  height: 55px;

  display: flex;
  align-items: center;
  justify-content: center;

  a {
    color: white;
    
    display: flex;
    align-items: center;


    img {
      height: 55px;
      margin-right: 10px;

    }
  }

  &:last-child {
    img {
      height: 35px;
    }
  }
}
</style>