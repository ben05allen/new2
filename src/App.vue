<template>
  <div class="flex flex-col bg-black min-h-screen font-Roboto">
    <SiteNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
    <router-view />
    <HiddenNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import { register } from 'swiper/element/bundle';
import SiteNav from "@/components/SiteNav.vue";
import HiddenNav from "@/components/HiddenNav.vue";

register();

const showMenu = ref(true);

const toggleMenu = () => {
    showMenu.value = !showMenu.value;
};
</script>
