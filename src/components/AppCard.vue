<script>
export default {
  props: { comics: Object },
};
</script>
<template>
  <section>
    <div class="card-container debug">
      <figure v-for="comic in comics" :key="comic.thumb">
        <img :src="comic.thumb" alt="" />
        <figcaption>{{ comic.series }}</figcaption>
      </figure>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

section {
  background-color: $main-bg;
  display: flex;
  justify-content: center;

  .card-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    width: 70%;
  }
  figure {
    width: 25%;
    gap: 2%;
  }
  img {
    max-width: 100%;
  }
}
</style>
