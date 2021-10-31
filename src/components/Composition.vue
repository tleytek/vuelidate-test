<template>
  <div class="hello">
    <input type="text" v-model="input" />
    <div>{{ input }} Without useVuelidate</div>
  </div>
</template>

<script>
import { ref } from "@vue/composition-api";

export default {
  setup() {
    const input = ref("");
    return { input };
  },
};
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
