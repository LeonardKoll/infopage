<template>
  <router-link
      class="inline-block w-20" v-for="item in menuItems" :key="item.title"
      :to="{'name': item.route}"
      >{{ item.title }}</router-link>
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
