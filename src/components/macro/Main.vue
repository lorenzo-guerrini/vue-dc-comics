<template>
  <main>
    <section>
      <div class="jumbotron"></div>
     </section>
     <section>
       <div class="container">
         <h2>Current Series</h2>
         <Comics />
         <button>Load More</button>
       </div>
     </section>
  </main>
</template>

<script>
import Comics from '../sections/Comics.vue'

export default {
  name: 'Main',
  components: {
    Comics
  }
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

section:last-of-type {
  font-family: 'Bangers', cursive;
}

.container {
  font-family: 'Bangers', cursive;
  
  flex-direction: column;
  align-items: flex-start;

  padding-bottom: 20px;

  h2 {
    font-size: 40px;
    background-color: $mainColor;
    padding: 10px 30px;

    transform: translate(0, -50%);
  }

  button {
    font-family: 'Bangers', cursive;
    font-size: 16px;

    padding: 10px 70px ;

    align-self: center;

    background-color: $mainColor;
  }
}
</style>
