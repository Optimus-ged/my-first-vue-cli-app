<template>
  <p class="todo-item" :class="{ 'is-complete': todo.completed }">
    <input type="checkbox" v-on:change="markComplete" />
    {{ todo.title }}
    <button class="del" @click="$emit('del-todo', todo.id)">x</button>
  </p>
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
  font-size: 13;
}
.is-complete {
  text-decoration: line-through;
}

.del {
  border-radius: 30px;
  height: 30px;
  width: 30px;
  background: #fa000f;
  float: right;
}
</style>