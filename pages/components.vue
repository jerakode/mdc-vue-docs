<template>
  <section class="container">
    <div>
      <mdc-checkbox v-if="isChecked" label="A Checkbox"></mdc-checkbox>
    </div>
    <div>
      <mdc-radio v-if="isRadio" label="Radio1" name="radios" value="radio1" v-model="picked" checked></mdc-radio>
      <mdc-radio v-if="isRadio" label="Radio2" name="radios" value="radio2" v-model="picked"></mdc-radio>
      <p>{{ picked }}</p>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      isChecked: false,
      isRadio: false,
      picked: null
    }
  },
  mounted () {
    this.isChecked = true
    this.isRadio = true
  }
}
</script>

<style lang="scss" scoped>
section {
  margin-top: 5em;
}
</style>
