<template>
  <section class="intro">
    <div class="container">
    <h1>VueJS wrapper arround Google's Material Components</h1>
    </div>
  </section>
</template>

<script>

export default {

}
</script>

<style lang="scss" scoped>
@import "~assets/styles/_variables.scss";

section {
  margin-top: 5em;
}

.intro {
  width: 100%;
  height: calc(100vh - 5em);
  background-color: $main-dark-color;
  color: $main-white-color;
}

h1 {
  font-size: 56px;
  font-weight: 400;
}
</style>
