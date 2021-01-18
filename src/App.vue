<template>
  <div>
    <Todos :todos="todos" />
  </div>
</template>

<script>
import Todos from "./components/todo";
export default {
  name : "App",
  components : {
    Todos
  },
  data(){
    return {
      todos : [
        {id : 1, title:"Home", complete:false},
        {id : 2, title:"Agents", complete:true},
        {id : 3, title:"Users", complete:false},
      ]
    }
  }
}
</script>

<style>
  *{
     box-sizing: border-box;
     margin: 0px;
     padding: 0px;
  }

  body{
    font-family: Arial, Helvetica, sans-serif;
  }
</style>