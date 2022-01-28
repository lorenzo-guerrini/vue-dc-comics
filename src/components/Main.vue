<template>
  <main>
    <div class="container">
      <section>
        <h1>--&gt; Content Goes here &lt;--</h1>
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Main'
}
</script>

<style scoped lang="scss">
@import "../assets/style/global.scss";
@import "../assets/style/partials/variables.scss";

main {
  background-color: $secondaryColor;
  color: white;
}

.container {
  font-family: 'Bangers', cursive;
  padding: 0 14px;

  height: 115px;
}
</style>
