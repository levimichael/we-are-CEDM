<template>
  <div class="we-are-cedm error">
    <h1>{{ msg }}</h1>
    <div class="background-rectangles"></div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'we are CEDM'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.we-are-cedm{
    display:flex;
    margin-left:10%;
}
h1{
  font-weight: normal;
  color: gray;
  display:inline;
  font-size: 20vw;
  line-height: .6;

}


.static {
  width: 100%;
  height: 100%;
  position: relative;
  margin: 0;
  padding: 0;
  top: -100px;
  opacity: 0.05;
  z-index: 230;
  user-select: none;
  user-drag: none;
}

.error {
  animation: noise 2s linear infinite;
  overflow: default;
}




.error:before {

  animation: noise-2 .2s linear infinite;
}

@keyframes noise {
  0%, 3%, 5%, 42%, 44%, 100% {opacity: 1; transform: scaleY(1);}
  4.3% {opacity: 1; transform: scaleY(1.7);}
  43% {opacity: 1; transform: scaleX(1.5); color: red;}
}


</style>
