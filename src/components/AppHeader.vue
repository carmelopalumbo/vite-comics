<script>
export default {
  name: "AppHeader",
  data() {
    return {
      menu: [
        {
          section: "characters",
          current: "false",
        },
        {
          section: "comics",
          current: "true",
        },
        {
          section: "movie",
          current: "false",
        },
        {
          section: "tv",
          current: "false",
        },
        {
          section: "games",
          current: "false",
        },
        {
          section: "collectibles",
          current: "false",
        },
        {
          section: "videos",
          current: "false",
        },
        {
          section: "fans",
          current: "false",
        },
        {
          section: "news",
          current: "false",
        },
        {
          section: "shop",
          current: "false",
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="logo" />
    <ul>
      <li v-for="(link, index) in menu" :key="index">
        {{ link.section }}
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixin" as *;
header {
  height: 117px;
  @include justify-between();
  width: 70%;
  margin: 0 auto;
  img {
    transform: scale(0.8);
  }
  ul {
    @include reset-list();
    li {
      @include reset-links();
    }
  }
}
</style>
