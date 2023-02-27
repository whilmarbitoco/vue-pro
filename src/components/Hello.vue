<template>
  <div>
    <h2>{{ msg}} </h2>
  </div>
</template>

<script>
export default {
  name: 'Hello',
  data() {
    return {
  msg: "hello world"
    }
  }
}
</script>

<style scoped>
div {
  color: red;
}
</style>
