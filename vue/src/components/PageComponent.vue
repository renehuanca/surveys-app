<script setup lang="ts">

interface Props {
    title?: string
}

const props = defineProps<Props>();

</script>

<template>
    <header class="bg-white shadow">
      <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold text-gray-900">
          {{ props.title }}
        </h1>
        <slot name="header"></slot>
      </div>
    </header>
    <main class="bg-gray-100">
      <div class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8 bg-gray-100">
        <!-- Replace with your content -->
        <div class="px-4 py-6 sm:px-0">
          <slot></slot>
        </div>
        <!-- /End replace -->
      </div>
    </main>
</template>