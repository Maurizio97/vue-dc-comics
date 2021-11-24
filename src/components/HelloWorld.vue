<template>
  <div class="hello">
    <h1>ciao</h1>
    <font-awesome-icon icon="user-secret"></font-awesome-icon>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

i {
  color: black;
}
</style>
