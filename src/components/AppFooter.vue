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
    <!-- FOOTER SITE INDEX -->
    <div class="footer-site-index">
      <div class="container">
        <div class="link-lists">
          <div class="col-list">
            <!-- DC links -->
            <span class="list-title">DC COMICS</span>
            <ul>
              <li v-for="comic in dcComics">
                <a :href="comic.url">{{ comic.text }}</a>
              </li>
            </ul>
            <!-- Shop links -->
            <span class="list-title">SHOP</span>
            <ul>
              <li v-for="shop in shops">
                <a :href="shop.url">{{ shop.text }}</a>
              </li>
            </ul>
          </div>
          <!-- DC links -->
          <div class="col-list">
            <span class="list-title">DC</span>
            <ul>
              <li v-for="dc in dcs">
                <a :href="dc.url">{{ dc.text }}</a>
              </li>
            </ul>
          </div>
          <!-- Sites links -->
          <div class="col-list">
            <span class="list-title">SITES</span>
            <ul>
              <li v-for="site in sites">
                <a :href="site.url">{{ site.text }}</a>
              </li>
            </ul>
          </div>
        </div>
        <!-- Big Logo -->
        <div class="big-logo">
          <img src="/img/dc-logo-bg.png" alt="big logo" />
        </div>
      </div>
    </div>
    <!-- Footer Social -->
    <div class="footer-social">
      <div class="container">
        <!-- Sign Up Button -->
        <div class="footer-sign-up">
          <button>SIGN-UP NOW!</button>
        </div>
        <!-- Social Links -->
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
@use "../styles/partials/variables" as *;

// FOOTER SITE INDEX
// Background image
.footer-site-index {
  background-image: url(img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 300px;
  display: flex;

  // Link lists
  .link-lists {
    display: flex;
    .col-list {
      display: flex;
      flex-direction: column;
      margin-right: 1.5rem;
    }
    .list-title {
      color: $text-color;
      font-size: 0.9rem;
    }
    ul {
      list-style-type: none;
      margin: 1rem 0;
      li {
        color: $text-muted;
        padding: 0.1rem 0;
        font-size: 11px;
      }
    }
  }

  // Big Logo
  .big-logo {
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

// Footer Social
.footer-social {
  background-color: $footer-bg;
  .footer-sign-up {
    margin: 1.5rem 0;
    padding: 0.8rem;
    border: 2px solid $brand-color;

    button {
      border-style: none;
      background-color: $footer-bg;
      color: $text-color;
      cursor: pointer;
    }
  }
  .footer-social-links {
    color: $text-color;
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
      color: $brand-color;
      font-weight: 600;
    }
  }
}
</style>
