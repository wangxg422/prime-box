<script setup lang="ts">
import { Button } from '@/components/ui/button';
import { Switch } from '@/components/ui/switch'

import { ref } from 'vue'
import { cn } from '@/lib/utils'
import { Slider } from '@/components/ui/slider'

const modelValue = ref([50])

</script>

<template>
  <main class="container">
    <div>
      <Button>Click me</Button>
    </div>
    <div>
      <Slider v-model="modelValue" :max="100" :step="1" :class="cn('w-3/5', $attrs.class ?? '')" />
    </div>
    <div>
      <Switch />
    </div>
  </main>
</template>

<style scoped></style>
<style>
:root {
  font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
  font-size: 16px;
  line-height: 24px;
  font-weight: 400;

  color: #0f0f0f;
  background-color: #f6f6f6;

  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  -webkit-text-size-adjust: 100%;
}

.container {
  margin: 0;
  padding: 0;
}

@media (prefers-color-scheme: dark) {
  :root {
    color: #f6f6f6;
    background-color: #2f2f2f;
  }

  a:hover {
    color: #24c8db;
  }

  input,
  button {
    color: #ffffff;
    background-color: #0f0f0f98;
  }

  button:active {
    background-color: #0f0f0f69;
  }
}
</style>