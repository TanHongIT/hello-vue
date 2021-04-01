<template>
  <div id="app">
    <!--root element -->
    <div v-show="isShow">
      <h1>lap trinh vien</h1>
    </div>

    <button @click="isShow = !isShow ">An/hien</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isShow: true,
    };
  },
};
</script>

<style>
</style>
