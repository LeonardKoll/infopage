<template>
    <div class="flex justify-between h-16">
      <div @click="$router.push({'name': 'Home'})" class="p-1 cursor-pointer">
        <img src="img/evorne_signet_black.svg" alt="Logo" class="h-14 inline"/>
        EVORNE
      </div>
      <div class="p-3">
        <TheMenu />
      </div>
    </div>
</template>

<script  lang="ts">
import { defineComponent } from 'vue'
import TheMenu from '@/components/TheMenu.vue'

export default defineComponent({
  components: {
    TheMenu
  }
})
</script>
