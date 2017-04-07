<template>
    <div id="app">
        <top></top>
        <router-view></router-view>
        <secondary></secondary>
    </div>
</template>

<script>
    import top from './components/Top.vue'
    import secondary from './components/Foot.vue'

    export default {
      name: 'app',
      components: {
         top,
         secondary
      }
    }
</script>

<style>
    body{
        margin:0;
        position:relative;
    }
    h1{
        color: white;
        font-size: 40pt;
        padding:0;
        margin:0;
    }
    a{
        text-decoration:none;
        color:white;
    }
    #app {
      font-family: 'Roboto', Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;
      color: #2c3e50;
    }
</style>
