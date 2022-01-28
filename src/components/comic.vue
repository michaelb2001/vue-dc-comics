<template>
<div class="container">
  <div class="comics" v-for="(element,index) in fumetti" :key="index"
    :thumb="element.thumb"
    :series="element.series"
  >
  </div>
</div>
</template>

<script>
export default {
  name: 'Comic',
  props: {
    thumb: String,
    price:String,
    series : String,
    type : String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
