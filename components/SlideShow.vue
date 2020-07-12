<template>
  <carousel :per-page="2" :pagenation-enabled="false">
    <slide :key="0">
      <p>1</p>
    </slide>
    <slide :key="1">
      <p>2</p>
    </slide>
    <slide :key="2">
      <p>3</p>
    </slide>
    <slide :key="3">
      <p>4</p>
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