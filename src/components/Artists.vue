<template>
  <div class="artist-grid">
        <div class="artist" v-for="artist in artists">
            <h3>{{artist.userName}}</h3>
        </div>
  </div>
</template>

<script>

//ADD CONTENTFUL HERE ONCE YOU FIGURE OUT THE API ;)

export default {
  name: 'artists',
  data () {
    return {
      mess: "hello",
      artists: [
          { userName: "Levi Whalen" },
          { userName: "Carlos Herrera" },
          { userName: "EMASOUND" },
          { userName: "Matthew Parker" },
          { userName: "Gui Brazil" },
          { userName: "GeekBoy" },
          { userName: "Edu Linares" },
          { userName: "Leandro Alencar" }

      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.artist-grid{
    display:flex;
    flex-wrap: wrap;
    width:80%;
    margin:auto;
}
.artist{
    display:flex;
    box-sizing: border-box;
    width:25%;
    background:white;
    padding:24px;
    height:240px;
}
@media only screen and (max-width: 768px) {
    .artist{
        width:50%;
    }
}
@media only screen and (max-width: 500px) {
    .artist{
        width:100%;
    }
}

</style>
