<template>
  <h3 class="todo-item" :class="{ 'is-complete': todo.completed }">
    <input type="checkbox" v-on:change="markComplete" />
    {{ todo.title }}
  </h3>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"],
  methods: {
    markComplete() {
      this.todo.completed = !this.todo.completed;
    },
  },
};
</script>

<style scoped>
.todo-item {
  background-color: white;
  border-bottom: grey dotted;
  padding: 10px;
}
.is-complete {
  text-decoration: line-through;
}
</style>