<script>
import { defineComponent } from 'vue';
import ColinlegInput from '@/colinlegInput.vue';

export default defineComponent({
  name: 'ServeDev',
  components: {
    ColinlegInput
  }
});
</script>

<template>
  <div id="app">
    <colinlegInput />
  </div>
</template>
