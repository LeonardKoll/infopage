<template>
  <div class="flex flex-col min-h-screen max-w-full bg-gray-100">
    <TheHeader class="flex-none"/>
    <router-view class="flex-auto" />
    <TheFooter class="flex-none"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import TheHeader from '@/components/TheHeader.vue'
import TheFooter from '@/components/TheFooter.vue'

export default defineComponent({
  components: {
    TheHeader,
    TheFooter
  }
})
</script>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>
