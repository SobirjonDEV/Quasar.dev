<template>
  <div class="row">
    <div class="col-8">
      <q-carousel
        v-model="slide"
        transition-prev="slide-right"
        transition-next="slide-left"
        animated
        control-color="white"
        navigation
        padding
        arrows
        infinite
        height="460px"
        class="bg-dark text-white "
      >
        <q-carousel-slide v-for="slide in slides" :key="slide" :name="slide.name" class="row column no-wrap flex-center">
          <div class="fit row wrap justify-center items-center content-center" >
            <div class="for_spacing col-10 text-h4 q-mt-lg" >
              {{slide.lorem}}
              <div class="row">
                <q-img
                  width="150px"
                  height="120px"
                  class="q-mt-xl"
                  :src="slide.img" />
                  <div class="q-mt-lg q-ml-xl"><br>
                    <span class="text-h4" style="letter-spacing: 3px;">{{slide.name_person}}</span><br>
                    <span class="text-subtitle1" style="letter-spacing: 3px;">CLIENT OF CLUB</span>
                  </div>
              </div>
            </div>
          </div>
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
      slide: ref('style'),
      slides:[
        {lorem:'Lorem ipsum dolor,  amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos',
        img:'https://avatars.mds.yandex.net/i?id=29aa7337015e6ad0083e2739abd59685-5316602-images-thumbs&n=13',
        name_person:'Night Wolf',
        name:1
        },
        {lorem:'Lorem ipsum dolor,  amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos',
        img:'https://avatars.mds.yandex.net/i?id=29aa7337015e6ad0083e2739abd59685-5316602-images-thumbs&n=13',
        name_person:'Night Wolf',
        name:2
        },
        {lorem:'Lorem ipsum dolor,  amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos',
        img:'https://avatars.mds.yandex.net/i?id=29aa7337015e6ad0083e2739abd59685-5316602-images-thumbs&n=13',
        name_person:'Night Wolf',
        name:3
        },

      ]
    }
  }
}
</script>
<style scoped>
</style>
