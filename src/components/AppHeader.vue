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
    <div class="debug">Logo</div>
    <div class="debug">
      <ul>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
        <li class="debug">ciao</li>
      </ul>
    </div>
  </header>
</template>
<style lang="scss" scoped>
@use "../styles/partials/mixins" as *;
header {
  @include flexed-on-line;
  height: 100%;
  ul {
    list-style-type: none;
    display: flex;
    li {
      padding: 0 1rem;
    }
  }
}
</style>
