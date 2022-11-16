<script>
export default {
  name: "AppCard",
  props: {
    card: Object,
  },
};
</script>

<template>
  <div class="card">
    <img :src="card.thumb" :alt="card.series" />
    <h4>{{ card.series }}</h4>
    <p>
      {{ card.price }} <br />
      BUY NOW!
    </p>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
.card {
  position: relative;
  width: calc(100% / 6);
  padding: 20px;
  cursor: pointer;
  img {
    width: 150px;
    height: 150px;
    object-fit: cover;
    object-position: top;
    transition: 0.4s all;
  }
  h4 {
    color: white;
    font-size: 0.85rem;
    padding: 10px 0;
    vertical-align: middle;
    display: inline-block;
    text-transform: uppercase;
  }
  p {
    text-align: center;
    position: absolute;
    top: 30%;
    left: 25%;
    opacity: 0;
    transition: 0.4s all;
    color: white;
    -webkit-text-stroke: 0.5px $secondary-color;
    font-weight: bold;
    font-size: 0.9rem;
  }
  &:hover p {
    opacity: 1;
  }
  &:hover img {
    filter: brightness(0.3);
  }
}
</style>
