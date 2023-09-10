<script>
export default {
  data() {
    return {
      rapidLinks: [
        {
          title: "DIGITAL COMICS",
          image: "/img/buy-comics-digital-comics.png",
          url: "#",
        },
        {
          title: "DC MERCHANDISE",
          image: "/img/buy-comics-merchandise.png",
          url: "#",
        },
        {
          title: "SUBSCRIPTION",
          image: "/img/buy-comics-subscriptions.png",
          url: "#",
        },
        {
          title: "DIGITAL COMICS",
          image: "/img/buy-comics-shop-locator.png",
          url: "#",
        },
        {
          title: "DC POWER VISA",
          image: "/img/buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>
<template>
  <div class="row">
    <div class="container-blue-row">
      <ul>
        <li v-for="rapidLink in rapidLinks">
          <span class="icon">
            <img :src="rapidLink.image" alt="" />
          </span>
          <a :href="rapidLink.url">
            <span class="title">{{ rapidLink.title }}</span>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
.row {
  background-color: #0c7cec;
  height: 150px;
  .container-blue-row {
    width: 70%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;

    ul {
      display: flex;
      justify-content: space-between;
      align-items: center;
      list-style-type: none;
    }
  }

  li {
    display: flex;
    align-items: center;
    padding: 1rem 2rem;
    .icon {
      display: flex;
      align-items: center;
      justify-content: center;
    }
    img {
      height: 50px;
      max-width: 50px;
    }

    .title {
      color: white;
      display: inline-block;
      margin-left: 1rem;
      font-size: 0.7rem;
    }
  }
}
</style>
