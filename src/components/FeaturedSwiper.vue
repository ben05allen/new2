<template>
    <div class="flex flex-col mt-36 bg-black items-center bg-yellow-200">
        
         <swiper 
            :spaceBetween="30"
            :centeredSlides="true"
            :autoplay="{
            delay: 5000,
            disableOnInteraction: false,
            }"
            :pagination="{
            clickable: true,
            }"
            :navigation="true"
            :modules="modules"
            class="mySwiper w-full py-12"
            >
            <swiper-slide>
                <img src="@/../public/feature_kitchen.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_batch.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_kitchen.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_batch.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            
        
        </swiper>

        <h3 class="text-white tracking-widest font-light lowercase text-center my-6 text-5xl">
            Featured Projects
        </h3>
    </div>
</template>

<script>

import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/navigation";



// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
    name: 'Featured',
    components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [ Autoplay, Pagination, Navigation],
    };
  },
};
</script>
