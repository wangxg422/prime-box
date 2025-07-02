<template>
    <ResizablePanelGroup id="demo-group-1" direction="horizontal" class="w-full h-screen">
        <ResizablePanel id="demo-panel-1" :default-size="30" :max-size="40" :min-size="20">
            <nav>
                <RouterLink to="/">Go to Home</RouterLink>
                <RouterLink to="/about">Go to About</RouterLink>
            </nav>
        </ResizablePanel>
        <ResizableHandle id="demo-handle-1" />
        <ResizablePanel id="demo-panel-2">
            <RouterView />
        </ResizablePanel>
    </ResizablePanelGroup>
</template>

<script setup lang="ts">
import {
    ResizableHandle,
    ResizablePanel,
    ResizablePanelGroup,
} from '@/components/ui/resizable'
</script>

<style scoped></style>