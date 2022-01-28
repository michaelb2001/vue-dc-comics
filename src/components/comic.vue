<template>
<div class="container">
    <img :src="comic.thumb">
    <p>{{comic.series}}</p>
</div>
</template>

<script>
export default {
  name: 'Comic',
  props: {
    comic: Object,
   
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/variables.scss';

.container{
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-content:center;
  width:200px;
  margin:40px;
  word-wrap : break;
  img{
    align-self: start;
  }
  p{
    color:$secondaryColor;
  }
}
</style>
