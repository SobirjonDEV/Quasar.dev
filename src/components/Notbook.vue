<template>
  <div>
      <div class="MyDiv ">
      <q-img
    class="MyNotbook"
    src="https://blanquette.qodeinteractive.com/wp-content/plugins/blanquette-core/inc/shortcodes/frame-slider/assets/img/frame-slider.png"
    alt="Frame slider phone">
      </q-img>
      <q-carousel
      animated
      v-model="slide"
      arrows
      infinite
      class="MyCarusel"
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
      </q-carousel>
    </div>
   </div>
</template>
<script>
import { ref } from 'vue'
export default {
  setup () {
    return {
      slide: ref(1),

    }
  }
}
</script>
<style scoped>
.MyCarusel{
  width: 78.5%;
  height: 345px;
  margin-left: 10.8%;
  margin-top: 1.5%;
  border-radius: 15px;
  position: absolute;
}
.MyNotbook{
  position: absolute;
}
.MyDiv{
  width: 50%;
  height: 50%;
  position: relative;
}
</style>
