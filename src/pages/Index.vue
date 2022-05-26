<template>
  <div>
    <!-- <carusel-dark/>
    <carusel-primary/>
    <swipercarusel/>
    <TikTokCarus/>
    <Notbook/>
    <UchcardCarus/>-->




   </div>
</template>
<script>
import { ref } from 'vue'
import CaruselDark from 'src/components/CaruselDark'
import CaruselPrimary from 'src/components/CaruselPrimary'
import Swipercarusel from 'src/components/Swipercarusel'
import TikTokCarus from '../components/TikTokCarus'
import Notbook from '../components/Notbook'
import UchcardCarus from '../components/UchcardCarus'
export default {
  components: {
    CaruselDark,
    CaruselPrimary,
    Swipercarusel,
    TikTokCarus,
    Notbook,
    UchcardCarus
},
     setup () {
    return {
      slide: ref(1),

    }
  }
}
</script>
<style scoped>


</style>
