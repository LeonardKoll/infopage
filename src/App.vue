<template>
  <div class="flex flex-col max-w-full border-4 border-indigo-600">
    <TheHeader class="flex-1"/>
    <router-view class="flex-1" />
    <TheFooter class="flex-1"/>
  </div>
</template>

<script>
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
