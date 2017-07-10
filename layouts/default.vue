<template>
  <div>
    <my-header/>
    <nuxt/>
  </div>
</template>

<script>
import MyHeader from '~components/Header.vue'

export default {
  components: {
    MyHeader
  }
}
</script>

<style lang="scss">
@import "~assets/styles/main.scss";

</style>
