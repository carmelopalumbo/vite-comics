<script>
// footer follow us
export default {
  name: "AppFooterBottom",
};
</script>

<template>
  <footer>
    <div class="content">
      <h4>SIGN-UP NOW!</h4>
      <div class="follow-us">
        <h4>FOLLOW US</h4>
        <img src="../assets/img/footer-facebook.png" alt="facebook" />
        <img src="../assets/img/footer-twitter.png" alt="twitter" />
        <img src="../assets/img/footer-youtube.png" alt="youtube" />
        <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
        <img src="../assets/img/footer-periscope.png" alt="periscope" />
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;

footer {
  height: 110px;
  background-color: lighten($primary-color, 8%);
  .content {
    @include justify-between();
    height: 100%;
    align-items: center;
    & > h4 {
      margin-left: 40px;
      padding: 13px;
      border: 2px solid $secondary-color;
      color: white;
      cursor: pointer;
    }
    .follow-us {
      display: flex;
      img {
        margin: 0 7px;
        cursor: pointer;
      }
      & > h4 {
        color: $secondary-color;
        margin-right: 30px;
        padding-top: 5px;
        font-size: 1.1rem;
      }
    }
  }
}
</style>
