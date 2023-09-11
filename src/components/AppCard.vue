<script>
export default {
  props: { comics: Object },
};
</script>
<template>
  <section>
    <div class="card-container">
      <figure v-for="comic in comics" :key="comic.thumb">
        <div class="card">
          <img :src="comic.thumb" alt="" />
        </div>

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
  padding: 2rem 0;
}

.card-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 0.5%;
  width: 70%;
}
.card {
  width: 160px;
  height: 170px;
  overflow: hidden;
}

figure {
  width: 16%;
  height: 16%;

  img {
    max-width: 100%;
  }

  figcaption {
    color: $text-color;
    font-size: 0.8rem;
    padding: 1rem 0;
  }
}
</style>
