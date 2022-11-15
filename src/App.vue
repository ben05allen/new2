<template>
  <div class="flex flex-col bg-black min-h-screen font-Roboto">
    <SiteNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
    <router-view />
    <HiddenNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
  </div>
</template>

<script>
import SiteNav from "@/components/SiteNav"
import HiddenNav from '@/components/HiddenNav'

export default {
  data() {
    return {
      showMenu: true
    }
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu
    }
  },
  components: {
    SiteNav,
    HiddenNav,
  },
}
</script>