<template>
  <div class="Menu">
    <span>{{ taskdata.content }}</span>
  </div>
</template>

<script>
export default {
  props: ["taskdata"],
  data() {
    return {
      content: "abc",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
