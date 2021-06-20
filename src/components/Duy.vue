<template>
  <div id="duy">
    <Scare v-bind:name="unit" />
    <button v-on:click="duyClick">Click</button>
  </div>
</template>

<script>
import Scare from './Scare.vue'
const duy = {
  name: 'Duy',
  data: () => {
    return {
      price: 10000
    }
  },
  props: {
    unit: String,
    msg: String,
  },
  methods: {
    duyClick: function () {
      this.$emit('keuGoiThayDOi')
    }
  },
  components: {
    Scare
  }
}
export default duy
</script>

<style scoped></style>
