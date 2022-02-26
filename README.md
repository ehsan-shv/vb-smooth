# vb-smooth

<a href="https://www.npmjs.com/package/vb-smooth"><img src="https://img.shields.io/npm/v/vb-smooth.svg" alt="Version"></a>

> Smooth scroll component for Vue3 and Nuxt apps. [Demo](https://ehsan-shv.github.io/vb-smooth/)

## Instalation

```bash
npm i vb-smooth
```

## Vue and Nuxt Example

```js
<template>
  <VBSmooth>
     // Your Content...
  </VBSmooth>
</template>
<script lang="ts">
import VBSmooth from 'vb-smooth';

export default {
  components: { VBSmooth },
};
</script>
```

## Vue and Vue Router Example

```js
<template>
  <VBSmooth>
    <router-view />
  </VBSmooth>
</template>
<script lang="ts">
import VBSmooth from 'vb-smooth';

export default {
  components: { VBSmooth },
};
</script>
```

## Customize

Check out options at [docs](https://github.com/idiotWu/smooth-scrollbar).

```js
<template>
  <VBSmooth :options="options">
    // Your Content...
  </VBSmooth>
</template>
<script lang="ts">
import { ref } from 'vue';
import VBSmooth from 'vb-smooth';

export default {
  components: { VBSmooth },
  setup() {
    const options = ref({
      // options
    });

    return {
      options,
    };
  },
};
</script>
```
