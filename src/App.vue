<template>
  <div>
    <h1>To-Do List</h1>
    <div>
      <TodoNew />
      <TodoList />
    </div>
  </div>
</template>
<script>

import TodoList from './components/TodoList.vue'
import TodoNew from './components/TodoNew.vue'
export default {
  components: {
    TodoNew,
    TodoList
  }
 
}
</script>
