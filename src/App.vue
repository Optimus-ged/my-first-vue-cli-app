<template>
  <Button :btn-text="text" :option="option" />
</template>

<script>
import Button from "./components/Button.vue";
export default {
  name: "App",
  components: {
    Button,
  },
  data: () => ({
    text: "Ouais ca marche",
    option: "tokos ",
  }),
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