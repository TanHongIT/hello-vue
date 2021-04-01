<template>
  <div id="app">
    <!--root element -->
    <div >
      <h1 :class="{daChon: selected}">lap trinh vien</h1>
       <button @click="selected = !selected">Doi mau</button> 

      <hr>
      <input type="text" :disabled="inputDisabled">
      <button @click="inputDisabled = !inputDisabled">Mo khoa</button> <!--chu y co : -->
    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      inputDisabled: true,
      selected: true,
    };
  },
};
</script>

<style>
.daChon{
  color: red;
}
</style>
