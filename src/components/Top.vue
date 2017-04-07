<template>
    <div class="top-bar">
    <h1><router-link to="/">we are <span class="CEDM">CEDM</span> </router-link></h1>
    <div class="nav-links">
         <router-link to="/artists">artists</router-link>
         <router-link to="/manifesto">manifesto</router-link>
         <router-link to="/events">events</router-link>
         <router-link to="/artist-resources">artist resources</router-link>
         <router-link to="/connect">connect</router-link>
    </div>
 </div>
</template>

<script>
export default {
  name: 'top',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.top-bar{
    width:100%;
    padding: 8px 24px;
    box-sizing: border-box;
    margin:auto;
    position:fixed;
    z-index:99;
    display:flex;
    justify-content:space-between;
    align-items: center;
    vertical-align: middle;
    background: #000046;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #1CB5E0, #000046);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #1CB5E0, #000046); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
.top-bar a{
    font-weight:100;
}
.top-bar h1 .CEDM{
    font-weight:900;
}
.nav-links{
    display: flex;
    width: 40%;
    justify-content: space-between;
}
</style>
