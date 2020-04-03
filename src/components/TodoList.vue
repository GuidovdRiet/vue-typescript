<template>
  <div>
    <h1>{{ title }}:</h1>
    <p>{{ typeTest }}</p>
    <ul v-for="todo in todos" v-bind:key="todo.id">
      <li>{{ todo.text }}</li>
    </ul>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  props: {
    typeTest: String
  },
  data() {
    return {
      title: "TODOS" as string,
      todos: [
        { text: "todo 1", done: false, id: Date.now() },
        { text: "todo 2", done: false, id: Date.now() + 1 }
      ] as Array<{ text: string; done: boolean; id: number }>
    };
  }
});
</script>

<style scoped></style>
