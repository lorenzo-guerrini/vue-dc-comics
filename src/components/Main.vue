<template>
  <main>
    <div class="container">
      <section>
        <strong>--&gt; Content Goes here &lt;--</strong>
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
</style>
