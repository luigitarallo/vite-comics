<script>
export default {};
</script>
<template>
  <main>
    <div class="series">CURRENT SERIES</div>
  </main>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;
main {
  background-image: url(../../public/img/jumbotron.jpg);
  height: 400px;
  position: relative;
}
.series {
  position: absolute;
  background-color: $brand-color;
  top: 94%;
  left: 14%;
  font-weight: 600;
  color: $text-color;
  padding: 0.8rem 2rem;
}
</style>
