<script>
export default {
  data() {
    return {};
  },
};
</script>
<template>
  <footer>
    <div></div>
    <div class="footer-site-links">
      <div class="container debug">
        <div class="site-links-list debug">
          <ul>
            li*3
          </ul>
          <ul>
            li*3
          </ul>
          <ul>
            li*3
          </ul>
        </div>
        <div class="logo-big">
          <img src="/img/dc-logo-bg.png" alt="big logo" />
        </div>
      </div>
    </div>
    <div></div>
  </footer>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;

.footer-site-links {
  background-image: url(img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 300px;

  .footer-site-links {
    display: flex;
  }
  .logo-big {
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;

    img {
      width: 450px;
    }
  }
}
</style>
