<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppBlueRaw from "./components/AppBlueRaw.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: { AppHeader, AppMain, AppBlueRaw, AppFooter },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppBlueRaw />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";

@import url("https://fonts.googleapis.com/css2?family=Libre+Franklin&family=Open+Sans:wght@500&display=swap");
</style>
