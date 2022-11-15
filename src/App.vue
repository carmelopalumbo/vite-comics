<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppJumbotron,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppJumbotron />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@100;300;400;700;900&display=swap");
</style>
