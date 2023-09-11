<script>
export default {
  props: { comics: Object },
};
</script>
<template>
  <section>
    <div class="card-gallery">
      <div class="card-container">
        <figure v-for="comic in comics" :key="comic.thumb">
          <div class="card">
            <img :src="comic.thumb" alt="" />
          </div>

          <figcaption>{{ comic.series }}</figcaption>
        </figure>
      </div>
    </div>
    <div class="button-container">
      <button>LOAD MORE</button>
    </div>
  </section>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

// Section
section {
  display: flex;
  flex-direction: column;
  background-color: $main-bg;
  padding: 2rem 0;
}
// Comics Card Gallery
.card-gallery {
  display: flex;
  justify-content: center;
}

.card-container {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 0.5%;
  width: 70%;
}
.card {
  height: 180px;
  width: 180px;
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

// Button load more

.button-container {
  display: flex;
  justify-content: center;

  button {
    margin-top: 1rem;
    border-style: none;
    padding: 0.5rem 3rem;
    color: $text-color;
    background-color: $brand-color;
    cursor: pointer;
  }
}
</style>
