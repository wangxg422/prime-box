<script setup lang="ts">
import {
  ResizableHandle,
  ResizablePanel,
  ResizablePanelGroup,
} from '@/components/ui/resizable'
</script>

<template>
  <main class="container">
    <ResizablePanelGroup id="demo-group-1" direction="horizontal" class="w-full h-screen">
      <ResizablePanel id="demo-panel-1" :default-size="30" :max-size="40" :min-size="20">
        Left
      </ResizablePanel>
      <ResizableHandle id="demo-handle-1" />
      <ResizablePanel id="demo-panel-2"  >
        Right
      </ResizablePanel>
    </ResizablePanelGroup>
  </main>
</template>

<style scoped></style>
<style>
:root {
  font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
  font-size: 16px;
  line-height: 24px;
  font-weight: 400;

  font-synthesis: none;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  -webkit-text-size-adjust: 100%;
}

.container {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100vh;
}
</style>