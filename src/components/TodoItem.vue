<template>
  <div class="todo-item" v-bind:class="{'is-complete':todo.completed}">
    <p>
      <input type="checkbox" v-on:change="markComplete"> 
      {{ todo.title }}
      <button @click="$emit('del-todo', todo.id)" class="del">x</button>
    </p>
    
  </div>
</template>

<script>
export default {
  name: 'TodoItem',
  props: ["todo"],
  methods: {
    markComplete() {
      this.todo.completed = !this.todo.completed;
    }
  }

}
</script>

<style scoped >
.todo-item {
  background-color: #f4f4f4;
  padding: 10px 25px;
  border-bottom: 1px dotted #ccc;
}
.todo-item input {
  margin-right: 12px;
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
  border-radius: 50%
}

</style>
