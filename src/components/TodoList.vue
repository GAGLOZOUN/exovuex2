<template>
 <div class="todos">
<ul>
  <li
    v-for="todo in todos"
    :key="todo.id"
  >
    {{ todo.task }}
  </li>
</ul>
</div>
</template>
<script>
export default {
  computed: {
    todos() {
      return this.$store.getters.getTodos;
    }
  }
};
</script>


<style scoped>

  .todos {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 1rem;
    border: 1px solid #ccc;
    background: #41b883;
  }
  
  
</style>