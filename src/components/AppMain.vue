<script>
export default {};
</script>
<template>
  <main>
    <div class="container">
      <p>--Contents goes here!--</p>
    </div>
  </main>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;
main {
  background-color: #1c1c1c;
  p {
    color: $text-color;
  }
  .container {
    height: 150px;
  }
}
</style>
