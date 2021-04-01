<template>
  <!--root element -->
  <div id="app">
    <div>
      <h1 :class="{ daChon: selected }">lap trinh vien</h1>
      <button @click="selected = !selected">Doi mau</button>

      <hr />
      <input type="text" :disabled="inputDisabled" />
      <button @click="inputDisabled = !inputDisabled">Mo khoa</button>
      <!--chu y co : -->
    </div>

    <hr />
    <div>
      <input type="text" v-model="changemane" />
      {{ changemane }}
    </div>
    
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputDisabled: true,
      selected: true,
      changemane: "Gau gau",
    };
  },
};
</script>

<style>
.daChon {
  color: red;
}
</style>
