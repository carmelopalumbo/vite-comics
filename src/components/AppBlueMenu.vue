<script>
// menu fascia blu
import menu from "../data/bluemenu.js";

export default {
  name: "AppBlueMenu",
  data() {
    return {
      menu,
    };
  },
  methods: {
    getPathImage(imageName) {
      return new URL(`../assets/img/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="menu-box">
    <div class="content">
      <ul>
        <li v-for="(link, index) in menu" :key="index">
          <img :src="getPathImage(link.img)" :alt="link.text" />
          <a href="#">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;
.menu-box {
  background-color: $secondary-color;
  height: 155px; //rimuovere
  .content {
    ul {
      @include reset-list();
      justify-content: space-between;
      li {
        display: flex;
        align-items: center;
        @include reset-links();
        img {
          transform: scale(0.5);
        }
        a {
          text-decoration: none;
          color: white;
          font-size: 0.9rem;
          font-weight: 300;
        }
      }
    }
  }
}
</style>
