<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  components: { AppHeader, AppFooter },
};
</script>

<template>
  <AppHeader />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";

@import url("https://fonts.googleapis.com/css2?family=Libre+Franklin&family=Open+Sans:wght@500&display=swap");
</style>
