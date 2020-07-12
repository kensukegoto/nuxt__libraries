<template>
  <carousel :per-page="2" :pagenation-enabled="false" class="slideshow">
    <slide :key="0" class="item">
      <div>
        100
      </div>
    </slide>
    <slide :key="1" class="item">
      <div>
        2
      </div>
    </slide>
    <slide :key="2" class="item">
      <div>
        3
      </div>
    </slide>
    <slide :key="3" class="item">
      <div>
        4
      </div>
    </slide>
  </carousel>
</template>

<script>
import Carousel from "vue-carousel/src/Carousel.vue";
import Slide from "vue-carousel/src/Slide.vue";

export default {
  components: {
    Carousel,
    Slide
  }
}
</script>

<style scoped>
.slideshow {
  width: 100%;
}
.item {
  width: 50%;
  background: aliceblue;
}
</style>