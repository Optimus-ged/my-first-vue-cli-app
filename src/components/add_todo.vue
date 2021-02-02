<template>
  <div>
      <form>
          <input type="text" name="title" placeholder="add a todo item ...">
          <input type="submit" value="Submit" class="btn">
      </form>
  </div>
</template>

<script>
export default {
    name:"addTodo"
}
</script>

<style scoped>
     form{
        display: flex;
    }

    input[type="text"]{
        flex: 10;
        padding: 5px;
        border: none;
        background-color: grey;
    }

    input[type="submit"]{
        flex: 5;
    } 

    .btn{
        border: none;
        background-color:#555;
        padding: 7px 20px;
    } 
    
</style>