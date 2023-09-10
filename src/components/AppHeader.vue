<script>
export default {
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          state: false,
        },
        {
          text: "COMICS",
          url: "#",
          state: true,
        },
        {
          text: "MOVIES",
          url: "#",
          state: false,
        },
        {
          text: "TV",
          url: "#",
          state: false,
        },
        {
          text: "GAMES",
          url: "#",
          state: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          state: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          state: false,
        },
        {
          text: "FANS",
          url: "#",
          state: false,
        },
        {
          text: "NEWS",
          url: "#",
          state: false,
        },
        {
          text: "SHOP",
          url: "#",
          state: false,
        },
      ],
    };
  },
};
</script>
<template>
  <header>
    <div class="container">
      <!-- Small Logo -->
      <div class="logo-small">
        <img src="img/dc-logo.png" alt="logo small" />
      </div>
      <!-- Nav -->
      <nav>
        <ul>
          <li v-for="link in links" :class="link.state ? 'link-selected' : ''">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>
<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;

// HEADER
header {
  background-color: $text-color;
}
// Small Logo
.logo-small {
  img {
    width: 5.5rem;
  }
}
// Navbar list
ul {
  display: flex;
  list-style: none;
  font-weight: 600;
  font-size: 0.8rem;

  li {
    padding: 3rem 0;
    margin-left: 2rem;
  }
}

.link-selected {
  color: $brand-color;
  border-bottom: 5px solid $brand-color;
}
</style>
