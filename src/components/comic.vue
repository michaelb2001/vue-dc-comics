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
  display:flex!important;
  flex-direction: column!important;
  align-items: center!important;
  justify-content:center!important;
  width:200px;
  margin:40px;
  word-wrap : break!important;
  text-align:center;

  img{
    align-self: start;
  }

  p{
    color:$secondaryColor;
  }
}
</style>
