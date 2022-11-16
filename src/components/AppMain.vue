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
    <h2 class>CURRENT SERIES</h2>
    <div class="content">
      <AppCard v-for="(card, index) in cards" :key="index" :card="card" />
    </div>
    <button>LOAD MORE</button>
  </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;
@use "../styles/general.scss" as *;

main {
  padding: 30px 0;
  h2 {
    width: 215px;
    transform: translateY(-50%);
    margin-left: 15%;
    text-align: center;
    color: white;
    padding: 7px 8px;
    background-color: $secondary-color;
    border: 1px solid $primary-color;
  }
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
  button {
    margin: 0 auto;
    display: block;
    @include buttons();
  }
}
</style>
