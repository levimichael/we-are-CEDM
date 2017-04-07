<template>
  <div id="app">
      <div class="top-bar">
      <h1><router-link to="/">we are CEDM</router-link></h1>
   <!-- use router-link component for navigation. -->
   <!-- specify the link by passing the `to` prop. -->
   <!-- <router-link> will be rendered as an `<a>` tag by default -->
   <router-link to="/artists">artists</router-link>
   <router-link to="/manifesto">manifesto</router-link>
   <router-link to="/events">events</router-link>
   <router-link to="/artist-resources">artist resources</router-link>
   </div>
    <router-view></router-view>
    <secondary></secondary>
  </div>
</template>

<script>
import secondary from './components/Foot.vue'

export default {
  name: 'app',
  components: {
     secondary
  }
}
</script>

<style>
body{
    background: #000046;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #1CB5E0, #000046);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #1CB5E0, #000046); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    margin:0;
}
h1{
    color: white;
    font-size: 60pt;
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
.top-bar{
    width:80%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items: center;
    vertical-align: middle;
}
</style>
