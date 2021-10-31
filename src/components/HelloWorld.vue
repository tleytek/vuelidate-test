<template>
  <div class="hello">
    Vue 2.6 + Composition API + Vuelidate 2
    <input type="text" v-model="input" />
    <div>{{ input }} With useVuelidate()</div>
  </div>
</template>

<script>
import { ref } from "@vue/composition-api";
import useVuelidate from "@vuelidate/core";
import { required } from "@vuelidate/validators";

export default {
  setup() {
    const input = ref("");
    const rules = { input: { required } };
    const v$ = useVuelidate(rules, { input });
    return { input, v$ };
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
