<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppBlueMenu from "./components/AppBlueMenu.vue";
import AppFooterTop from "./components/AppFooterTop.vue";
import AppFooterBottom from "./components/AppFooterBottom.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppBlueMenu,
    AppFooterTop,
    AppFooterBottom,
  },
};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppBlueMenu />
  <AppFooterTop />
  <AppFooterBottom />
</template>

<style lang="scss">
@use "./styles/general.scss";
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@100;300;400;700;900&display=swap");
</style>
