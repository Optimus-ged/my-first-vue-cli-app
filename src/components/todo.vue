<template>
  <div>
    <div :key="todo.id" v-for="todo in todos">
      <TodoItem :todo="todo" />
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
