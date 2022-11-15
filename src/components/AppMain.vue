<script>
export default {
  name: "AppMain",
};
</script>

<template>
  <main>
    <div class="container">
      <h1>CONTENTS HERE...</h1>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;

main {
  background-color: $primary-color;
  height: 120px; //rimuovere
  .container {
    @include content();
    h1 {
      color: white; //rimuovere
    }
  }
}
</style>
