<template>
  <div id="scare">
    <h1>{{ name }}</h1>
  </div>
</template>

<script>
export default {
  name: 'scare',
  data: () => {
    return { }
  },
  props: {
    name: String
  },
}
</script>

<style scoped>
  #scare {
    border: 1px solid;
    margin: 10px;
  }
</style>
