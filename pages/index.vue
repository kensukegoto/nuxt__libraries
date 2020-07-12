<template>
  <div class="container">
    <slideShow />
    <vueSwiper />
  </div>
</template>

<script>
import SlideShow from '~/components/SlideShow.vue';
import VueSwiper from '~/components/VueSwiper.vue'

export default {
  components: {
    SlideShow,
    VueSwiper
  }
}
</script>
