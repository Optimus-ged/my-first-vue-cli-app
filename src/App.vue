<template>
  <div>
    <Todo :todos="todos" v-on:del-todo="deleteTodo" />
  </div>
</template>

<script>
import Todo from "./components/todo";
export default {
  name: "App",
  components: {
    Todo,
  },
  data() {
    return {
      todos: [
        { id: 1, title: "Home Page", completed: false },
        { id: 2, title: "Users", completed: false },
        { id: 3, title: "Products", completed: false },
        { id: 4, title: "About", completed: false },
        { id: 5, title: "Exit", completed: false },
      ],
    };
  },
  methods: {
    deleteTodo(id) {
      this.todos = this.todos.filter((todo) => todo.id !== id);
    },
  },
};
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>