<template>
  <div class="comic">
      <a href="#">
          <div class="comic-thumb">
            <img :src="comic.thumb" :alt="comic-series">
          </div>
          <div class="comic-series">
          {{comic.series}}
          </div>
      </a>
  </div>
</template>

<script>
export default {
    name: 'Comic',
    props: {
        comic: Object
    }
}
</script>

<style scoped lang="scss">
@import "../../assets/style/global.scss";
@import "../../assets/style/partials/variables.scss";

.comic {
    height: 262px;
    width: 210px;

    padding: 0 12px;

    a {
        color: white;
    }

    .comic-thumb {
        height: 175px;

        text-align: center;

        overflow: hidden;

        img {
            width: 175px;
        }
    }

    .comic-series {
        margin: 15px 5.5px;
    }
}
</style>