<script>
// main
import AppCard from "./AppCard.vue";
import cards from "../data/dc-comics";

export default {
  name: "AppMain",
  components: {
    AppCard,
  },
  data() {
    return {
      cards,
    };
  },
};
</script>

<template>
  <main>
    <div class="jumbotron">
      <img src="../assets/img/jumbotron.jpg" alt="jumbotron" />
    </div>
    <div class="content">
      <AppCard v-for="(card, index) in cards" :key="index" :card="card" />
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;
@use "../styles/general.scss" as *;

main {
  background-color: $primary-color;
  .jumbotron img {
    height: 400px;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }
  .content {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>
