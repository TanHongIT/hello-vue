<template>
  <!--root element -->
  <div id="app">
    <Task v-for="(task, index) in tasks" :key="index" :taskdata="task"/>
    <hr>
    <TagSelector/>
  </div>
</template>

<script>
import Task from './components/Task';
import TagSelector from './components/TagSelector';
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
    Task,
    TagSelector
  }
};
</script>

<style>

</style>
