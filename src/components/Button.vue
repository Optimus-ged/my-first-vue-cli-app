<template>
  <Button class="my-btn">{{ btnText }}</Button>
</template>

<script>
export default {
  props: ["btnText"],
};
</script>

<style scoped>
    .my-btn{
        background-color: red;
        padding: 100px;
    }
</style>