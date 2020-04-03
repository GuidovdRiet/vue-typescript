<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <TodoForm />
    <TodoList v-bind:typeTest="123" />
  </div>
</template>

<script>
// @ is an alias to /src
import TodoForm from "@/components/TodoForm.vue";
import TodoList from "@/components/TodoList.vue";

export default {
  name: "Home",
  components: {
    TodoForm,
    TodoList
  }
};
</script>
