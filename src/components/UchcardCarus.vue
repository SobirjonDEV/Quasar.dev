<template>
  <div>
     <div style="width:80%;">
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
      height="350px"
      class="bg-grey-1 shadow-2 rounded-borders"
    >
      <q-carousel-slide v-for="slide in slides " :key="slide" :name="slide.name" class="column no-wrap animate__animated animate__backInRight">
        <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
          <q-card v-for="card in cards" :key="card" class="my-card">
            <img :src="card.src">
              <q-card-section>
                  <div class="text-h6">Our Changing Planet</div>
                  <div class="text-subtitle2">by John Doe</div>
              </q-card-section>
          </q-card>
        </div>
      </q-carousel-slide>

    </q-carousel>
  </div>
  </div>
</template>
<script>
import { ref } from 'vue'

export default {
  setup() {
    return{
      slide: ref(1),
      slides:[
        {name:1,},
        {name:2,},
      ],
      cards:[
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
        {src:'https://cdn.quasar.dev/img/mountains.jpg'},
      ]
    }
  }
}
</script>
<style lang="">

</style>
