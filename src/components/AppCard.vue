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
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6);
  padding: 20px;
  cursor: pointer;
  img {
    width: 150px;
    height: 150px;
    object-fit: cover;
    object-position: top;
  }
  h4 {
    color: white;
    font-size: 0.85rem;
    padding: 10px 0;
    vertical-align: middle;
    display: inline-block;
    text-transform: uppercase;
  }
}
</style>
