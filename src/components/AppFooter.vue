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
    <div class="footer-social debug">
      <div class="container">
        <div class="footer-sign-up">
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="footer-social-links">
          <ul>
            <li><span class="social-claim">FOLLOW US</span></li>
            <li><img src="/img/footer-facebook.png" alt="" /></li>
            <li><img src="/img/footer-twitter.png" alt="" /></li>
            <li><img src="/img/footer-youtube.png" alt="" /></li>
            <li><img src="/img/footer-pinterest.png" alt="" /></li>
            <li><img src="/img/footer-periscope.png" alt="" /></li>
          </ul>
        </div>
      </div>
    </div>
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
.footer-social {
  background-color: #303030;
  .footer-sign-up {
    margin: 1.5rem 0;
    padding: 0.8rem;
    border: 2px solid #0c7cec;

    button {
      border-style: none;
      background-color: #303030;
      color: white;
      cursor: pointer;
    }
  }
  .footer-social-links {
    color: white;
    ul {
      display: flex;
      list-style-type: none;
      align-items: center;
      li {
        margin-left: 1rem;
      }
      .social-claim {
        color: #0c7cec;
        font-weight: 600;
      }
    }
  }
}
</style>
