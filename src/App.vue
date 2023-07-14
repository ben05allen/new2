<template>
  <div class="flex flex-col bg-black min-h-screen font-Roboto">
    <SiteNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
    <router-view />
    <HiddenNav :showMenu="showMenu" @menu-toggle="toggleMenu()" />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { register } from 'swiper/element/bundle';
import SiteNav from "@/components/SiteNav"
import HiddenNav from '@/components/HiddenNav'

register();

const showMenu = ref(true);

const toggleMenu = () => {
    showMenu.value = !showMenu.value;
};
</script>
