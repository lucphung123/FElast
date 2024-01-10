<template>
  <swiper :modules="modules" :slides-per-view="1" autoplay :pagination="{ clickable: true }" :scrollbar="{ draggable: true }">
    <swiper-slide v-for="(product, index) in products" :key="index">
      <div class="flex justify-center items-center mx-20 my-20">
        <div class="xl:mt-0 space-y-8 flex-col justify-center items-center ml-4 text-white">
          <p class="font-600 text-7xl">{{product.name }}</p>
          <p class="text-3xl">{{ product.office }}</p>
        </div>
        <div class="h-full rounded-5 flex justify-center items-center p-7">
          <img class="rounded-5" :src="product.src" alt="" />
        </div>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue"
import { EffectCards, Autoplay, Navigation } from "swiper"
import "swiper/css"
import "swiper/css/effect-cards"
import "swiper/css/navigation"
import "swiper/css/autoplay"

const modules = [EffectCards, Autoplay, Navigation]
const products = [
  {
    src: "/1.jpg",
    name: "EduBook",
    office: "Cội nguồn của tri thức",
  },
  {
    src: "/1.jpg",
    name: "EduBook",
    office: "Cội nguồn của tri thức",
  },
]
let mySwiper = ref({})
const setSwiper = xswiper => {
  mySwiper.value = xswiper
}
</script>

<style scoped>
.swiper-slide-content {
  display: flex;
  flex-direction: column;
}
</style>
