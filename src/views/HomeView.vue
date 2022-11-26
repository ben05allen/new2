<template>
  <div id="home">
    <Featured />
    
  </div>
</template>

<script>

import Featured from '@/components/FeaturedSwiper.vue'
import Project from '@/components/ProjectSwiper.vue'

export default {
  name: 'home',
  components: {
    Featured,
    Project,
  }
}
</script>
