<template>
  <div class="wrapper">
    <nav>Navigation</nav>
    <div class="content">
      <div class="sidebar">sidebar</div>
      <main>main</main>
    </div>
    
  </div>
</template>

<script>
// javascript
export default {
  name: "App",
  components: {},
  data: () => ({}),
};
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

.wrapper {
  background-color: #35363a;
  height: 100vh;
  widows: 100vw;
  position: relative;
}

nav{
  height: 70px;
  width: 100vw;
  background-color: red;
  position: fixed;
  top: 0;
  z-index: 100;
}

.content{
  display: flex;
  margin-top: 70px;
}

.sidebar{
  height: calc(100vh - 70px);
  width: 400px;
  background-color: green;
  position: fixed;
  top: 70px;
}

main{
  height: 1000px;
  flex-basis: calc((100vw - 400px));
  background-color: aquamarine;
  margin-left: 400px;  
}
</style>