<template>
  <div class="container">
    <div class="header">
        <img src="../assets/img/dc-logo.png" id="logo_header" alt="DC logo">

        <nav>
          <ul>
            <li v-for="(element,index) in navList" :key="index">
              <a href="#" :class="{'active' : element.current}">{{element.name}}</a>
            </li>
          </ul>
        </nav>
    </div>
  </div>
</template>

<script>


export default {
  name: 'Header',
  data(){
    return {
      navList : [
        {
          "name" : "CHARACTERS",
          'current' : false
        },
        {
          "name" : "COMICS",
          'current' : true
        },
        {
          "name" : "MOVIES",
          'current' : false
        },
        {
          "name" : "TV",
          'current' : false
        },
        {
          "name" : "GAMES",
          'current' : false
        },
        {
          "name" : "COLLECTIBLES",
          'current' : false
        },
        {
          "name" : "VIDEO",
          'current' : false
        },
        {
          "name" : "FANS",
          'current' : false
        },
        {
          "name" : "NEWS",
          'current' : false
        },
        {
          "name" : "SHOP",
          'current' : false
        }
        
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';



.header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
  img{
    height: 80px;
    margin: 20px 0px;
  }
  nav{
    height: 100%;

  ul{
      list-style-type: none;
      height: 100%;
      li{
        display: inline-block;
        margin: 0 5px;
        height: 100%;
        a{
          display:inline-block;
          text-decoration: none;
          text-transform: uppercase;
          color: $mainColor;
          height: 100%;
        }
      }
    }
  }
  
}

.active{
  border-bottom: 5px solid $activeColor;
}
</style>
