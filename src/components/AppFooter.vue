<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <footer>
    <div class="content">
      <h3>SIGN-UP NOW!</h3>
      <div class="follow-us">
        <h3>FOLLOW US</h3>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/general.scss" as *;
@use "../styles/partials/mixin" as *;

footer {
  height: 110px;
  background-color: lighten($primary-color, 10%);
}
</style>
