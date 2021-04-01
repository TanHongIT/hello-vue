<template>
  <!--root element -->
  <div id="app">
    <Task v-for="(task, index) in tasks" :key="index"/>
  </div>
</template>

<script>
import Task from './components/Task';
export default {
  data(){
    return{
      tasks: [
        { content: "di choi", done: false },
        { content: "nau an", done: false },
        { content: "code", done: false },
        { content: "di ve sinh", done: false },
      ]
    }
  },
  components:{
    Task
  }
};
</script>

<style>

</style>
