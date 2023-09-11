<script>
export default {};
</script>
<template>
  <main>
    <div class="container"></div>
  </main>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;
main {
  background-image: url(../../public/img/jumbotron.jpg);
  p {
    color: $text-color;
  }
  .container {
    height: 400px;
  }
}
</style>
