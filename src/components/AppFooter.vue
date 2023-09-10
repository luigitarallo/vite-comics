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

      dcComics: [
        { text: "Characters", url: "#" },
        { text: "Comics", url: "#" },
        { text: "Movies", url: "#" },
        { text: "TV", url: "#" },
        { text: "Games", url: "#" },
        { text: "Videos", url: "#" },
        { text: "News", url: "#" },
      ],

      shops: [
        { text: "Shop DC", url: "#" },
        { text: "Shop DC Collectibles", url: "#" },
      ],

      dcs: [
        { text: "Terms Of Use", url: "#" },
        { text: "Privacy policy(New)", url: "#" },
        { text: "Ad Choices", url: "#" },
        { text: "Advertising", url: "#" },
        { text: "Jobs", url: "#" },
        { text: "Subscriptions", url: "#" },
        { text: "Talent Workshops", url: "#" },
        { text: "CPSC Certificates", url: "#" },
        { text: "Ratings", url: "#" },
        { text: "Shop Help", url: "#" },
        { text: "Contact Us", url: "#" },
      ],

      sites: [
        { text: "DC", url: "#" },
        { text: "MAD Magazine", url: "#" },
        { text: "DC Kids", url: "#" },
        { text: "DC Universe", url: "#" },
        { text: "DC Power Visa", url: "#" },
      ],
    };
  },
};
</script>
<template>
  <footer>
    <div></div>
    <div class="footer-site-links">
      <div class="container">
        <div class="site-links-lists">
          <div class="col-1-link">
            <div class="site-link-title">
              <span>DC COMICS</span>
              <ul>
                <li v-for="comic in dcComics">
                  <a :href="comic.url">{{ comic.text }}</a>
                </li>
              </ul>
            </div>
            <div class="site-link-title">
              <span>SHOP</span>
              <ul>
                <li v-for="shop in shops">
                  <a :href="shop.url">{{ shop.text }}</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-2-link">
            <div class="site-link-title">
              <span>DC</span>
              <ul>
                <li v-for="dc in dcs">
                  <a :href="dc.url">{{ dc.text }}</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-2-link">
            <div class="site-link-title">
              <span>SITES</span>
              <ul>
                <li v-for="site in sites">
                  <a :href="site.url">{{ site.text }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="logo-big">
          <img src="/img/dc-logo-bg.png" alt="big logo" />
        </div>
      </div>
    </div>
    <div class="footer-social">
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
  display: flex;

  .site-links-lists {
    display: flex;
    .col-1-link {
      display: flex;
      flex-direction: column;
      margin-right: 1rem;
    }
    .col-2-link {
      margin-right: 1rem;
    }

    .site-link-title {
      color: white;
      margin-top: 1rem;
    }
    ul {
      margin-right: 1rem;
      margin-top: 0.7rem;
      margin-bottom: 0.7rem;
      color: white;
      list-style-type: none;
      font-size: 12px;
      li {
        color: rgb(162, 162, 162);
        padding: 0.1rem 0;
      }
    }
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
