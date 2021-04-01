<template>
  <!--root element -->
  <div id="app">
    {{tongtien | dauphancach}}
    <button @click="tongtien+=20000">add</button>
  </div>
</template>

<script>
export default {
  data(){
    return{
      tongtien: 1000000
    }
  },
  filters:{
    dauphancach: function(sotien){
      return sotien.toFixed(2).replace(/\d(?=(\d{3})+\.)/g, '$&,');
    }
  }
};
</script>

<style>

</style>
