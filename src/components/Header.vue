<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="DC">
      </div>
      <nav>
        <ul>
          <li>a</li>
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
      currentItem: 0
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
