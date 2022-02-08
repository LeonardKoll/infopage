<template>
  <div class="flex items-center h-10 w-96 bg-white shadow-md rounded-full">
    <router-link
      class="flex-auto text-center h-10 p-1 rounded-full border-4 border-white"
        v-for="item in menuItems" :key="item.title"
        :to="{'name': item.route}"
        >{{ item.title }}
      </router-link>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

var menuItems = [
  {
    icon: '',
    title: 'Home',
    route: 'Home'
  }, {
    icon: '',
    title: 'About',
    route: 'About'
  }, {
    icon: '',
    title: 'Preview',
    route: 'Preview'
  }
]

export default defineComponent({
  data () {
    return {
      menuItems
    }
  }
})
</script>

<style scoped>
@layer components {
  .router-link-active {
    @apply bg-red-500;
  }
}
</style>
