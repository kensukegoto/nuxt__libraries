<template>
  <carousel 
  :per-page="1" 
  :pagenation-enabled="false" 
  :perPageCustom="[[600, 2], [960, 3]]" 
  class="slideshow">
    <slide :key="0" class="item">
      <figure class="item__image">
        <img src="/image/event_10.jpg" alt="">
      </figure>
      <div class="item__meta">
        <p class="item__meta__state">受付中</p>
        <p class="item__meta__date"><i class="far fa-calendar"></i>2020.1.10</p>
        <p class="item__meta__locate"><i class="fas fa-map-marker-alt"></i>渋谷</p>
      </div>
      <p class="item__title">フォームのバリデーションをしてみよう</p>
      <a class="item__link"></a>
    </slide>
    <slide :key="1" class="item">
      <figure class="item__image">
        <img src="/image/event_09.jpg" alt="">
      </figure>
      <div class="item__meta">
        <p class="item__meta__state">受付中</p>
        <p class="item__meta__date"><i class="far fa-calendar"></i>2020.1.9</p>
        <p class="item__meta__locate"><i class="fas fa-map-marker-alt"></i>渋谷</p>
      </div>
      <p class="item__title">ページネーションを作成してみよう</p>
      <a class="item__link"></a>
    </slide>
    <slide :key="2" class="item">
      <figure class="item__image">
        <img src="/image/event_08.jpg" alt="">
      </figure>
      <div class="item__meta">
        <p class="item__meta__state">受付中</p>
        <p class="item__meta__date"><i class="far fa-calendar"></i>2020.1.8</p>
        <p class="item__meta__locate"><i class="fas fa-map-marker-alt"></i>渋谷</p>
      </div>
      <p class="item__title">アコーディオンで実装するよくある質問を作ってみよう</p>
      <a class="item__link"></a>
    </slide>
    <slide :key="3" class="item">
      <figure class="item__image">
        <img src="/image/event_07.jpg" alt="">
      </figure>
      <div class="item__meta">
        <p class="item__meta__state">受付中</p>
        <p class="item__meta__date"><i class="far fa-calendar"></i>2020.1.7</p>
        <p class="item__meta__locate"><i class="fas fa-map-marker-alt"></i>渋谷</p>
      </div>
      <p class="item__title">タブとを実装しよう</p>
      <a class="item__link"></a>
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

<style lang="scss" scoped>
$breakpoints: (
  's' : 'screen and (max-width: 374px)',
  'm' : 'screen and (min-width: 560px)',
  'l' : 'screen and (min-width: 960px)',
) !default;

@mixin media($breakpoint: l) {
  @media #{map-get($breakpoints,$breakpoint)}{
    @content;
  }
}

.slideshow {
  width: 100%;
}
.item {

  position: relative;
  width: 50%;
  
  &__meta {
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 1.2rem;
    background-color: #f1f1f1;
    &__state{
      display: flex;
      justify-content: center;
      align-items: center;
      height: 56px;
      width: 33.3333%;
      max-width: 80px;
      background-color: #22b1ed;
      color: #fff;
    }
    &__locate {
      padding-right: 20px;
    }
    .far,.fas {
      margin-right: 8px;
    }
  }

  &__title{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 16px;
    font-weight: bold;
    line-height: 1.6;
    background: #fff;
    height: 80px;
  }

  &__link {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #fff;
    opacity: 0;
    transition: opacity .2s;
  }
  &:hover &__link{
    opacity: .3;
  }

  img {
    max-width: 100%;
    vertical-align: bottom;
  }
}
</style>