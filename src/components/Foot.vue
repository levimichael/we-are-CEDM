<template>
    <div class="footer-wrap">
        <div class="footer-content">
            <p>Supported by prayers and funded by the community on Patreon.com </p>
            <div class="language-select">
                <p>English | Español</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'secondary',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer-wrap{
    background: #000046;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #1CB5E0, #000046);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #1CB5E0, #000046); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    position: fixed;
    z-index:99;
    bottom:0;
    display: block;
    width:100%;
}
.footer-content{
    display:flex;
    justify-content:space-between;
    width:80%;
    margin:auto;
    color:rgba(255, 255, 255, 0.31);
}
.language-select{
    background: black;
    padding: 0 20px;
    color:white;
}

</style>
