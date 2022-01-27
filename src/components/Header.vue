<template>
  <div class="container">
    <div class="header">
        <img src="../assets/img/dc-logo.png" id="logo_header" alt="DC logo">

        <nav>
          <ul>
            <li><a href="#">CHARACTERS</a></li>
            <li><a href="#" class="active">COMICS</a></li>
            <li><a href="#">MOVIES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">GAMES</a></li>
            <li><a href="#">CHARACTERS</a></li>
            <li><a href="#">COLLECTIBLES</a></li>
            <li><a href="#">VIDEO</a></li>
            <li><a href="#">FANS</a></li>
            <li><a href="#">NEWS</a></li>
            <li><a href="#">SHOP</a></li>
          </ul>
        </nav>
    </div>
  </div>
</template>

<script>


export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';



.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  min-height: 100px;
  img{
    height: 80px;
  }

  ul{
    list-style-type: none;
    li{
      display: inline;
      margin: 0 5px;

      a{
        text-decoration: none;
        color: $mainColor;
      }
    }
  }
}





</style>
