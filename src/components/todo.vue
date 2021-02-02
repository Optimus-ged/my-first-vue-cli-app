<template>
  <div>
    <div :key="todo.id" v-for="todo in todos">
      <TodoItem :todo="todo" v-on:del-todo="$emit('del-todo', todo.id)"/>
    </div>
  </div>
</template>

<script>
import TodoItem from "./todo_item";
export default {
  name: "Todo",
  components: {
    TodoItem,
  },
  props: ["todos"],
};
</script>
