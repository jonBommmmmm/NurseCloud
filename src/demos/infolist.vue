<template>
  <div>
    <myheader></myheader>
    <div style="height: 100%;padding-top: 101px; ">
      <p v-for="i in 100">{{i}}</p>
    </div>
  </div>
</template>
<script>
  import myheader from './infolistheader.vue'
  export default {
    components: {
      myheader
    }
  }
</script>
<style>
</style>
