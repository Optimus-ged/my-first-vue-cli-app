<template>
  <h3 class="todo-item">{{ todo.title }}</h3>
</template>

<script>
export default {
  name:"TodoItem",
  props:["todo"]
}
</script>

<style scoped>
  .todo-item{
    background-color: white;
    border-bottom: grey dotted;
    padding: 10px;
  }
</style>