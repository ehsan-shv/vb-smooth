<template>
  <div id="smooth-layer">
    <slot />
  </div>
</template>

<script lang="ts">
import { defineComponent, onMounted, nextTick } from 'vue';
import Scrollbar from 'smooth-scrollbar';

export default defineComponent({
  name: 'SmoothScroll',
  props: {
    options: {
      type: Object,
    },
  },

  setup(props) {
    const setSmoothScroll = (container: HTMLElement | null) => {
      if (container) Scrollbar.init(container, props.options);
    };

    onMounted(() => {
      nextTick(() => {
        const container = document.getElementById('smooth-layer');
        setSmoothScroll(container);
      });
    });
  },
});
</script>

<style>
html {
  overflow: hidden !important;
}

#smooth-layer {
  position: fixed !important;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}
</style>
