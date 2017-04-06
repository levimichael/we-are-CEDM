<template>
  <div class="users">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'users',
  data () {
    return {
      msg: 'these are users'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

</style>
