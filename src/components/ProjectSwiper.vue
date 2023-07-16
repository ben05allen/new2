<template>
    <div class="flex flex-col mt-36 bg-black items-center">
        
         <swiper-container
            :spaceBetween="10"
            :navigation="true"
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
        </swiper-container>
        <swiper-container
            :spaceBetween="10"
            :slidesPerView="4"
            :freeMode="true"
            :watchSlidesProgress="true"
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
        </swiper-container>
        <h3 class="text-white tracking-widest font-light lowercase text-center my-6 text-5xl">
            Featured Projects
        </h3>
    </div>
</template>
