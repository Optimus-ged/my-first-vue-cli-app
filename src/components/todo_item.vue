<template>
  <div class="todo-item">
    <p>{{ todo.title }}</p>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"],
  components: {},
};
</script>

<style>
.todo-item {
  padding: 10px;
  background: white;
  border-bottom: pink dotted;
}
</style>