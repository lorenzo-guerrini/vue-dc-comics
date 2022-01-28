<template>
  <section>
    <!-- sx -->
    <div>
      <button>Sign-up now!</button>
    </div>

    <!-- dx -->
    <div>
      <span>Follow us</span>
      <ul>
        <li v-for="(social, i) in socials" :key="i">
          <a :href="social.url">
            <img :src="require('../assets/img/' + social.icon)" :alt="social.name">
          </a>
        </li>
      </ul>
      
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/global.scss";
@import "../assets/style/partials/variables.scss";

</style>
