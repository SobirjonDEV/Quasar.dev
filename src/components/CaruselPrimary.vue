<template>
  <div>
    <div style="width:90%;">
       <q-carousel
        v-model="slide"
        transition-prev="scale"
        transition-next="scale"
        swipeable
        animated
        control-color="dark"
        arrows
        padding
        navigation
        infinite
        height="300px"
        class="bg-white text-dark shadow-3"
      >
      <q-carousel-slide name="style" class="text-dark column no-wrap flex-center">
            <div class=" q-mt-lg text-center text-h4 text-weight-thin">
              <span>OUR CLIENTS WORLDS</span>
            </div>
              <div class="fit row wrap justify-center items-start content-start">
                <q-avatar size="150px" class="shadow-10 q-mt-sm">
                  <img src="https://avatars.mds.yandex.net/i?id=12ead51e206bc04bb14c3ba0c5e9ba4e-5873671-images-thumbs&n=13" alt="">
                </q-avatar>
                <div style="width:80%;" class="full-height q-mt-sm">
                  <span class="column q-ml-xl q-mt-md text-weight-regular text-italic text-h6">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit, unde blanditiis! Quo modi aperiam dolore placeat, voluptatum iste consectetur praesentium temporibus voluptatem neque sunt accusantium, totam expedita sint! Eos, possimus.
                  </span>
                </div>
              </div>
          <div class="full-width row justify-end">
                <span class=" q-mr-xl text-grey text-h6">
                  Night Wolf SkyKing
                </span>
          </div>
      </q-carousel-slide>
      <q-carousel-slide name="TV" class="text-dark column no-wrap flex-center">
            <div class=" q-mt-lg text-center text-h4 text-weight-thin">
              <span>OUR CLIENTS WORLDS</span>
            </div>
              <div class="fit row wrap justify-center items-start content-start">
                <q-avatar size="150px" class="q-mt-sm">
                  <img src="https://avatars.mds.yandex.net/i?id=12ead51e206bc04bb14c3ba0c5e9ba4e-5873671-images-thumbs&n=13" alt="">
                </q-avatar>
                <div style="width:80%;" class="full-height q-mt-sm">
                  <span class="column q-ml-xl q-mt-md text-weight-regular text-italic text-h6">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit, unde blanditiis! Quo modi aperiam dolore placeat, voluptatum iste consectetur praesentium temporibus voluptatem neque sunt accusantium, totam expedita sint! Eos, possimus.
                  </span>
                </div>
              </div>
          <div class="full-width row justify-end">
                <span class=" q-mr-xl text-grey text-h6">
                  Night Wolf SkyKing
                </span>
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

    }
  }
}
</script>
<style scoped>

</style>
