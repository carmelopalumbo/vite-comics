<script>
export default {
  name: "AppMain",
};
</script>

<template>
  <main>
    <div class="content">
      <h1>CONTENTS HERE...</h1>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixin" as *;
@use "../styles/general.scss" as *;

main {
  background-color: $primary-color;
  height: 120px; //rimuovere
  .content {
    h1 {
      color: white; //rimuovere
      text-align: center; //rimuovere
      padding-top: 30px; //rimuovere
    }
  }
}
</style>
