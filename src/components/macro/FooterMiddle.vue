<template>
  <section>
    <div class="container">
      <div class="category" v-for="(category, i) in categories" :key="i">
        <h3>{{category.text}}</h3>
        <ul>
          <li v-for="(item, p) in category.items" :key="p">
            <a :href="item.url">{{item.text}}</a>
          </li>
        </ul>
      </div>

      <div id="dc-logo-bg">
        <img src="../../assets/img/dc-logo-bg.png" alt="DC">
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FooterMiddle',
  data() {
    return{
      categories: [
        {
          text: "Dc Comcs",
          items: [
            {
              text: "Characters",
              url: "#"
            },
            {
              text: "Comics",
              url: "#"
            },
            {
              text: "Movies",
              url: "#"
            },
            {
              text: "TV",
              url: "#"
            },
            {
              text: "Games",
              url: "#"
            },
            {
              text: "Videos",
              url: "#"
            },
            {
              text: "News",
              url: "#"
            }
          ]
        },
        {
          text: "Shop",
          items: [
            {
              text: "Shop DC",
              url: "#"
            },
            {
              text: "Shop DC Colectibles",
              url: "#"
            }
          ]
        },
        {
          text: "DC",
          items: [
            {
              text: "Terms Of Use",
              url: "#"
            },
            {
              text: "Privacy policy (new)",
              url: "#"
            },
            {
              text: "Ad Choices",
              url: "#"
            },
            {
              text: "Advertising",
              url: "#"
            },
            {
              text: "Jobs",
              url: "#"
            },
            {
              text: "Subscriptions",
              url: "#"
            },
            {
              text: "Talent Workshops",
              url: "#"
            },
            {
              text: "CPSC Certificates",
              url: "#"
            },
            {
              text: "Ratings",
              url: "#"
            },
            {
              text: "Shop Help",
              url: "#"
            },
            {
              text: "Contact Us",
              url: "#"
            }
          ]
        },
        {
          text: "Sites",
          items: [
            {
              text: "DC",
              url: "#"
            },
            {
              text: "MAD Magazine",
              url: "#"
            },
            {
              text: "DC Kids",
              url: "#"
            },
            {
              text: "DC Universe",
              url: "#"
            },
            {
              text: "DC Power Visa",
              url: "#"
            }
          ]
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../../assets/style/global.scss";

section {
  background-image: url("../../assets/img/footer-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;

  overflow: hidden;
}

.container {
  padding: 40px 14px 50px;
  
  align-items: flex-start;
  flex-wrap: wrap;

  font-family: 'Bangers', cursive;

  position: relative;
}

.category {
  padding-right: 30px;

  h3 {
    font-size: 26px;
    color: white;

    margin-bottom: 10px
  }

  li {
    font-size: 13px;

    margin: 4px 0;

    a {
      color: #959595;
    }
  }
}

#dc-logo-bg {
  position: absolute;

  top: -100px;
  right: 0px;
}
</style>
