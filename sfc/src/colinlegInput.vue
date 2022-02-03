<template>
  <div>
    <input ref="input" v-model="input" @blur="restart" type="text" placeholder="my-component" class="myInput">
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default /*#__PURE__*/defineComponent({
  name: 'ColinlegInput', // vue component name
  data(){
    return {
      input: null
    }
  },
  methods: {
    restart() {
      this.$refs.input.value = ""
    }
  }
});
</script>



<style scoped>
  .colinlegInput {
    display: block;
    width: 400px;
    margin: 25px auto;
    border: 1px solid #ccc;
    background: #eaeaea;
    text-align: center;
    padding: 25px;
  }
  .colinlegInput p {
    margin: 0 0 1em;
  }

  .myInput {
    border: 5px solid #4893bd;
    border-radius: 3px;
    box-shadow: #9c8f8f 3px 3px;
    outline: none;
    padding: 10px;
  }
</style>
