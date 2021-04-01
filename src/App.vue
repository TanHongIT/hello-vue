<template>
  <div id="app">
    <!--root element -->
    <div >
      <h1 :id="id">lap trinh vien</h1>
      <input type="text" :disabled="inputDisabled">
      <button @click="inputDisabled = !inputDisabled">Mo khoa</button> <!--chu y co : -->
    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      id: 'gaugau',
      inputDisabled: true
    };
  },
};
</script>

<style>
</style>
