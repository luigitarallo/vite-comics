<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <div class="wrapper">
    <nav class="debug">
      <div class="container debug">
        <AppHeader />
      </div>
    </nav>
  </div>
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
