<template>
  <div>
    <div class="q-mt-xl ">
      <q-carousel
        animated
        v-model="slide"
        infinite
        arrows
        class="MyCarusel rotate-90"
        transition-prev="slide-right"
        transition-next="slide-left"
        @mouseenter="autoplay = false"
        @mouseleave="autoplay = true"
      >
        <q-carousel-slide v-for="slide in slides" :key="slide" :name="slide.name" class="MySlide">
          <q-video
          :src="slide.src"
          style="height:100%;"
          />
        </q-carousel-slide>
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
      slides:[
        {src:'https://www.youtube.com/embed/MmdKeypSxE8',name:1},
        {src:'https://www.youtube.com/embed/MmdKeypSxE8',name:2},
        {src:'https://www.youtube.com/embed/MmdKeypSxE8',name:3},
        {src:'https://www.youtube.com/embed/MmdKeypSxE8',name:4},
      ]

    }
  }
}
</script>
<style scoped>
.MyCarusel{
  width: 500px;
  height: 500px;
}
.MySlide{
  transform: rotate(270deg);
}
</style>
