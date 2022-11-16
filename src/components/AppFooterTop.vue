<script>
// footer con menu list
export default {
  name: "AppFooterTop",
};
</script>

<template>
  <div class="jumbotron">
    <div class="content">
      <div>
        <h4>DC COMICS</h4>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <h4>SHOP</h4>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>

      <div>
        <h4>DC</h4>
        <ul>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>

      <div>
        <h4>SITES</h4>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <img src="../assets/img/dc-logo-bg.png" alt="" class="bglogo" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;
@use "../styles/partials/media";

.jumbotron {
  height: 370px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  .content {
    position: relative;
    overflow: hidden;
    display: flex;
    div {
      padding: 30px;
      h4 {
        padding: 10px 0;
        color: white;
        font-size: 1.1rem;
      }
    }
    ul {
      list-style: none;
      a {
        text-decoration: none;
        color: #959595;
        font-size: 0.75rem;
        display: inline-block;
        padding: 5px 0;
        &:hover {
          text-decoration: underline;
        }
      }
    }
  }
  .bglogo {
    position: absolute;
    top: -80px;
    right: 0;
  }
}
</style>
