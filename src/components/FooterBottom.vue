<template>
  <section>
    <div class="container">
      <!-- sx -->
      <div>
        <button>Sign-up now!</button>
      </div>

      <!-- dx -->
      <div id="footer-bottom-dx">
        <span>Follow us</span>
        <ul>
          <li v-for="(social, i) in socials" :key="i">
            <a :href="social.url">
              <img :src="require('../assets/img/' + social.icon)" :alt="social.name">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FooterBottom',
  data() {
    return{
      socials: [
        {
          name: "Facebook",
          url: "#",
          icon: "footer-facebook.png"
        },
        {
          name: "Twitter",
          url: "#",
          icon: "footer-twitter.png"
        },
        {
          name: "You Tube",
          url: "#",
          icon: "footer-youtube.png"
        },
        {
          name: "Pinterest",
          url: "#",
          icon: "footer-pinterest.png"
        },
        {
          name: "Periscope",
          url: "#",
          icon: "footer-periscope.png"
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/style/global.scss";
@import "../assets/style/partials/variables.scss";

section {
  background-color: $tertiaryColor;
}

.container {
  padding: 30px 14px;

  justify-content: space-between;

  font-family: 'Bangers', cursive;
}

button {
  font-family: 'Bangers', cursive;
  font-size: 20px;
  color: white;

  padding: 12px;

  background: none;

  border: 2px solid $mainColor;

  cursor: pointer;
}

#footer-bottom-dx {
  display: flex;
  align-items: center;

  span {
    font-size: 26px;
    padding-right: 10px;

    color: $mainColor;
  }

  ul {
    display: flex;

    li {
      margin-left: 15px;
    }
  }
}

</style>
