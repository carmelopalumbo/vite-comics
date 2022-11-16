<script>
// header con menu
import menu from "../data/menu.js";

export default {
  name: "AppHeader",
  data() {
    return {
      menu,
    };
  },
};
</script>

<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="logo" />
    <ul>
      <li v-for="(link, index) in menu" :key="index">
        <a href="">{{ link.section }}</a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixin" as *;
@use "../styles/partials/variables" as *;
header {
  height: 117px;
  @include justify-between();
  width: 70%;
  margin: 0 auto;
  img {
    transform: scale(0.8);
    cursor: pointer;
  }
  ul {
    @include reset-list();
    li {
      @include reset-links();
      a {
        color: lighten($primary-color, 15%);
        text-decoration: none;
        padding-bottom: 43px;
        &:hover {
          box-shadow: 0px 7px 0px 0px lighten($secondary-color, 10%);
        }
      }
    }
  }
}
</style>
