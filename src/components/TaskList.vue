<template>
  <div class="task">
    <span>{{ taskData.content }}</span>
  </div>
</template>

<script>
export default {
  props: ['taskData'],
  data() {
    return {
      content: "abc",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
