<template>
  <div>
    <!-- <carusel-dark/>
    <carusel-primary/>
    <swipercarusel/>
    <TikTokCarus/>
    <Notbook/>-->
<a target="blanck" href="https://preview.themeforest.net/item/industo-factory-business-html-template/full_screen_preview/37634265?_ga=2.122449739.1724580808.1652354433-1887451697.1651578636&_gac=1.219625707.1652354758.Cj0KCQjw4PKTBhD8ARIsAHChzRJy2jUitxTxvq8PgySZL2r4v5QD99xCOq0wZ7C0ZW2wntH-xlSTTEAaAi9lEALw_wcB">;oojdf</a>
  <!-- <div style="width:80%;">
     <q-carousel
      v-model="slide"
      transition-prev="slide-right"
      transition-next="slide-left"
      swipeable
      animated
      infinite
      control-color="primary"
      padding
      arrows
      height="300px"
      class="bg-grey-1 shadow-2 rounded-borders"
    >
      <q-carousel-slide v-for="slide in slides " :key="slide" :name="slide.name" class="column no-wrap">
        <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
          <q-img class="rounded-borders col-4 full-height" :src="slide.src" />
          <q-img class="rounded-borders col-4 full-height" :src="slide.src1" />
          <q-img class="rounded-borders col-4 full-height" :src="slide.src2" />

        </div>
      </q-carousel-slide>

    </q-carousel>
  </div> -->




   </div>
</template>
<script>
import { ref } from 'vue'
import CaruselDark from 'src/components/CaruselDark'
import CaruselPrimary from 'src/components/CaruselPrimary'
import Swipercarusel from 'src/components/Swipercarusel'
import TikTokCarus from '../components/TikTokCarus'
import Notbook from '../components/Notbook'
export default {
  components: {
    CaruselDark,
    CaruselPrimary,
    Swipercarusel,
    TikTokCarus,
    Notbook
},
     setup () {
    return {
      slide: ref(1),
      slides:[
        {name:1,src:'https://cdn.quasar.dev/img/mountains.jpg',src1:'https://cdn.quasar.dev/img/parallax1.jpg',src2:'https://cdn.quasar.dev/img/parallax1.jpg'},
        {name:2,src:'https://cdn.quasar.dev/img/mountains.jpg',src1:'https://cdn.quasar.dev/img/parallax1.jpg',src2:'https://cdn.quasar.dev/img/parallax1.jpg'},
        {name:3,src:'https://cdn.quasar.dev/img/mountains.jpg',src1:'https://cdn.quasar.dev/img/parallax1.jpg',src2:'https://cdn.quasar.dev/img/parallax1.jpg'},
        {name:4,src:'https://cdn.quasar.dev/img/mountains.jpg',src1:'https://cdn.quasar.dev/img/parallax1.jpg',src2:'https://cdn.quasar.dev/img/parallax1.jpg'},

      ]

    }
  }
}
</script>
<style scoped>


</style>
