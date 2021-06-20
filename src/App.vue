<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Duy v-bind:unit="unit"  msg="Alo ALo!" v-on:keuGoiThayDOi="changeUnit"/>
  </div>
</template>

<script>
import Duy from './components/Duy.vue'

export default {
  name: 'App',
  data: () => ({
    unit: 'aaa',
    scarest: [{
      name: 'Dipe'
    }, {
      name: 'ChuThang'
    }, {
      name: 'AQuan'
    }, {
      name: 'Co'
    }]
  }),
  methods: {
    changeUnit: function () {
      this.unit = 'bbbbb'
    }
  },
  components: {
    Duy,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
