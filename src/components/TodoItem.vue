<template>
  <div>
    <p>Todo item</p>
  </div>
</template>

<script>
export default {
  name: 'TodoItem'
}
</script>

<style scoped >
.todo-item {
  background-color: #f4f4f4;
  padding: 10px;
  border-bottom: 1px dotted #ccc;
}
.is-complete {
  text-decoration: line-through;
}
.del {
  background-color: #ff0000;
  color: #fff;
  border: none;
  padding: 5px 9px;
  cursor: pointer;
  float: right;
}

</style>
