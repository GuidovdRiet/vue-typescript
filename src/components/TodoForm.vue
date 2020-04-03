<template>
  <form v-on:submit="pressMe">
    <input placeholder="insert" />
    <button type="submit">submit</button>
  </form>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "TodoForm",
  props: {
    msg: String
  },
  data() {
    return {
      test: "Hello" as string
    };
  },
  methods: {
    pressMe(): string {
      return this.test;
    }
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
