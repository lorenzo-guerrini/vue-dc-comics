<template>
  <header>
    <div class="container">
      <div class="logo">
        <a href="#">
          <img src="../assets/img/dc-logo.png" alt="DC">
        </a>
      </div>
      <nav>
        <ul>
          <li v-for="(item, i) in menuItems" :key="i">
            <a :href="item.url" :class="{'active': currentItem == i}">{{item.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      menuItems: [
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
          text: "Collectibles",
          url: "#"
        },
        {
          text: "Videos",
          url: "#"
        },
        {
          text: "Fans",
          url: "#"
        },
        {
          text: "News",
          url: "#"
        },
        {
          text: "Shop",
          url: "#"
        }
      ],
      currentItem: 1
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/global.scss";
@import "../assets/style/partials/variables.scss";

.container {
  justify-content: space-between;

  height: 115px;

  padding: 0 15px;
}

.logo {
  a {
    display: flex;
    align-items: center;

    img {
      height: 81px;
      width: 81px;
    }
  }
}

ul {
  display: flex;

  li {
    padding: 0 10px;
  }
} 

</style>
