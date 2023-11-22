<template>
  <div class="absolute top-0 w-full">
    <swiper
      :slidesPerView="1"
      :spaceBetween="30"
      :loop="true"
      :pagination="{
        clickable: true,
      }"
      :navigation="true"
      :modules="modules"
      class="mySwiper" 
      >
      <SwiperSlide> <img class="w-screen" src="@/assets/images/sliders/slider1.jpg" alt="" srcset="" /> </SwiperSlide>
      <SwiperSlide> <img class="w-screen" src="@/assets/images/sliders/slider2.jpg" alt="" srcset="" /> </SwiperSlide>
      <SwiperSlide> <img class="w-screen" src="@/assets/images/sliders/slider3.jpg" alt="" srcset="" /> </SwiperSlide>
      <SwiperSlide> <img class="w-screen" src="@/assets/images/sliders/slider4.jpg" alt="" srcset="" /> </SwiperSlide>
    </swiper>
  </div>

  <div class=" relative">
    <h1 v-for="item in 20" :key="item">
      {{ item }} askjdfsak fsak lksadjsak lakdsd ask
    </h1>
  </div>
  
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

// import required modules
import { Pagination, Navigation } from "swiper/modules";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
    };
  },
};
</script>
