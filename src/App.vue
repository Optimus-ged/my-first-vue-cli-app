<template>
  <div>
    <Todo :todos="todos"/>
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
        { id: 1, title: "home", completed: true },
        { id: 2, title: "Users", completed: false },
        { id: 3, title: "Settings", completed: true },
      ],
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>

