<script lang="ts">
import { defineComponent } from 'vue';
import VbSmooth from '@/vb-smooth.vue';

export default defineComponent({
  name: 'ServeDev',
  components: {
    VbSmooth
  }
});
</script>

<template>
  <div id="app">
    <vb-smooth />
  </div>
</template>
