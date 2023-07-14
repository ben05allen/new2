<template>
    <div class="flex flex-col mt-36 bg-black items-center">
         <swiper-container 
            :spaceBetween="30"
            :centeredSlides="true"
            :autoplay="{
                delay: 5000,
                reverse: true
            }"
            :pagination="{
                clickable: true,
            }"
            :navigation="true"
            class="mySwiper w-full py-12"
            >
            <swiper-slide>
                <img src="@/../public/feature_kitchen.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_batch.webp" class="w-full object-cover" alt="Living the dream">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_kitchen.webp" class="w-full object-cover" alt="Designer Kitchen">
            </swiper-slide>
            <swiper-slide>
                <img src="@/../public/feature_batch.webp" class="w-full object-cover" alt="Living the dream">
            </swiper-slide>
        </swiper-container>

        <h3 class="text-white tracking-widest font-light lowercase text-center my-6 text-5xl">
            Featured Projects
        </h3>
    </div>
</template>

