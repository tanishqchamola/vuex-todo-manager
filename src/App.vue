<template>
  <div>
    <h1 style="text-align: center">Vuex Todo Manager</h1>
    <div class="container">
      <div class="row">
        <AddTodo />
      </div>
      <div class="row">
        <FilterTodo />
      </div>
      <div class="row">
        <Todos />
      </div>
    </div>
  </div>
</template>

<script>
import Todos from "@/components/Todos.vue";
import AddTodo from "@/components/AddTodo.vue";
import FilterTodo from "@/components/FilterTodo.vue";
export default {
  name: "app",
  components: {
    Todos,
    AddTodo,
    FilterTodo
  }
};
</script>

<style>
body {
  font-family: "Open Sans", Arial, sans-serif;
  line-height: 1.6;
  background-color: #e8f7f0;
}
.container {
  max-width: 1100px;
  margin: auto;
  overflow: auto;
  padding: 0 2rem;
}
.row {
  margin-top: 10px;
  margin-bottom: 15px;
}
</style>