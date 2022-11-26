<template>
    <div class="flex flex-col mt-36 bg-black items-center">
        
         <swiper 
            :spaceBetween="10"
            :navigation="true"
            :thumbs="{ swiper: thumbsSwiper }"
            :modules="modules"
            class="mySwiper2"
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
        <swiper
            @swiper="setThumbsSwiper"
            :spaceBetween="10"
            :slidesPerView="4"
            :freeMode="true"
            :watchSlidesProgress="true"
            :modules="modules"
            class="mySwiper"
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
import "swiper/css/free-mode";



// import required modules
import { FreeMode, Thumbs, Navigation } from "swiper";

export default {
    name: 'Project',
    components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    let thumbsSwiper = null;

    const setThumbsSwiper = (swiper) => {
      thumbsSwiper = swiper;
    }

    return {
      modules: [FreeMode,Navigation,Thumbs],
    };
  }
};
</script>
