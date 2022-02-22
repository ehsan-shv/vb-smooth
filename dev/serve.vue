<script lang="ts">
import { defineComponent } from 'vue';
import VbSmooth from '@/vb-smooth.vue';

export default defineComponent({
  name: 'ServeDev',
  components: {
    VbSmooth,
  },
});
</script>

<template>
  <div id="app">
    <vb-smooth>
      <div class="container">
        <h1>Hello World!</h1>
        <h2>Smooth Scroll</h2>
        <h3>Vue App</h3>
      </div>
    </vb-smooth>
  </div>
</template>

<style>
.container {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  height: 500vh;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
</style>
