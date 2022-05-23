<template>
  <swiper
    :slidesPerView="5"
    :spaceBetween="30"
    :centeredSlides="true"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper bg-dark"
  >
    <swiper-slide  v-for="slide in slides" :key="slide" style="margin-top:35px ">
     <q-card class="my-card">
      <img :src="slide.src">
        <q-card-section>
          <div class="text-h6">Our Changing Planet</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>
      </q-card>
    </swiper-slide>

  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
// import required modules
import { Pagination } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination],
      slides:[
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},

      ]
    };
  },
};

</script>
<style scoped>
.mySwiper{
  height:330px;
}
</style>
