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
          { userName: "Levi Whalen",
            genre: "trance"
          },
          { userName: "Carlos Herrera",
            genre: "everything"
          },
          { userName: "EMASOUND" },
          { userName: "Matthew Parker" },
          { userName: "Gui Brazil" },
          { userName: "GeekBoy" },
          { userName: "Edu Linares" },
          { userName: "Leandro Alencar" },
          { userName: "Chris Howland" },
          { userName: "Neon Feather" },
          { userName: "GV3" },
          { userName: "Reyer" },
          { userName: "Wiilky" }

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
    width:100%;
    z-index:50;
    position:relative;
    overflow:hidden;
    justify-content: space-between;
}
.artist{
    display:flex;
    box-sizing: border-box;
    width:22%;
margin-top:40px;
    background:white;
    padding:24px;
    height:240px;
    position:inherit;
    background: #8e9eab;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #eef2f3, #8e9eab);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #eef2f3, #8e9eab); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

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
