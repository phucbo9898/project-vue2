<template>
  <div id="app">
    <Task v-for="(task, index) in tasks" :key="index" :taskData="task" />
  </div>
</template>

<script>
import Task from "./components/TaskList.vue";
export default {
  data() {
    return {
      tasks: [
        { content: "đi chợ", done: false },
        { content: "code", done: false },
        { content: "nấu ăn", done: false },
        { content: "đi chơi", done: false },
      ],
    };
  },
  components: {
    Task,
  },
};
</script>

<style>
.completed {
  text-decoration: line-through;
  color: red;
}
</style>
