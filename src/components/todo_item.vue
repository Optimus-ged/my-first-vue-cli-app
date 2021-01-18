<template>
    <div class="tod-item">
        <p>{{ todo.title }}</p>
    </div>
</template>

<script>
export default {
    name : "TodoItem",
    props : ["todo"]
}
</script>

<style scoped>
    .tod-item{
        padding: 10px;
        background: white;
        border-bottom: 1px dotted white;
    }
</style>