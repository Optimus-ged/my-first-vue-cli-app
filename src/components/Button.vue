<template>
  <div>
    <h1>{{ option }}</h1>
    <Button class="my-btn">{{ btnText }}</Button>
  </div>
</template>

<script>
export default {
  props: ["btnText", "option"],
};
</script>

<style scoped>
.my-btn {
  background-color: red;
  padding: 20px;
}
</style>