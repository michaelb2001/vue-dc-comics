<template>
<div class="contenitore">
  <div class="container">
    <p>&larr;Content Here&rarr;</p>
  </div>
</div>

</template>

<script>
export default {
  name: 'Main',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variables.scss';


.contenitore{
  width: 100%;
  background-color: $mainColor;

  .container{
    display: flex;
    align-items: center;
    justify-content: start;
    min-height: 100px;
    font-size: $fontx2;
    padding: 20px;

    p{
      color: $secondaryColor;
    }
  }
}

</style>
