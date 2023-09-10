<script>
export default {
  data() {
    return {
      sociaLinks: [
        {
          text: "facebook",
          icon: "/img/footer-facebook.png",
          url: "#",
        },
        {
          text: "twitter",

          icon: "/img/footer-twitter.png",
          url: "#",
        },
        {
          text: "youtube",
          icon: "/img/footer-youtube.png",
          url: "#",
        },
        {
          text: "pinterest",

          icon: "/img/footer-pinterest.png",
          url: "#",
        },
        {
          text: "periscope",
          icon: "/img/footer-periscope.png",
          url: "#",
        },
      ],
    };
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
          <div><span class="social-claim">FOLLOW US</span></div>
          <ul>
            <li v-for="socialLink in sociaLinks">
              <a :href="socialLink.url"
                ><img :src="socialLink.icon" alt="facebook icon"
              /></a>
            </li>
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
    display: flex;
    align-items: center;
    ul {
      display: flex;
      list-style-type: none;
      align-items: center;
      li {
        margin-left: 1rem;
      }
    }
    .social-claim {
      color: #0c7cec;
      font-weight: 600;
    }
  }
}
</style>
