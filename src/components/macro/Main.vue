<template>
  <main>
    <section>
      <div class="jumbotron"></div>
     </section>
     <section>
       <div class="container">
         <h2>Current Series</h2>
       </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<style scoped lang="scss">
@import "../../assets/style/global.scss";
@import "../../assets/style/partials/variables.scss";

main {
  background-color: $secondaryColor;
  color: white;
}

.jumbotron {
  background-image: url("../../assets/img/jumbotron.jpg");
  background-size: cover;
  height: 265px;
}

.container {
  font-family: 'Bangers', cursive;
  padding: 0 14px;
}
</style>
