# 参考

- https://github.com/vuejs/awesome-vue#carousel
- https://www.to-r.net/media/nuxt-setup/

# scss

https://www.npmjs.com/package/@nuxtjs/style-resources

# スライドショー

- vue carousel
- vue-awesome-swiper
- swiper
- slick

## vue carousel

無限ループ出来ない。矢印では可能だがスワイプでの無限ループに対応していない。

## vue-awesome-swiper

### 困った

- コンポーネントで作ると下記エラー
- コンポーネントでなんとか作ろうと client-only にするとSSRされない（当然…）

### 参考

- [swiper公式](https://swiperjs.com/api/)
- [vue-awesome-swiper公式](https://www.npmjs.com/package/vue-awesome-swiper)
- [コンポーネントで作る お手本](https://qiita.com/nakanishi03/items/c12221be7645b84016c8)
- [ディレクティブで作る お手本](https://web-niar.com/blog/nuxt-js-vue-awesome-swiper/)

# コミット

```
追加：vue-carouselのインストール、プラグインとして読む
追加：スライドショーのコンポーネントを作成
追加：もくもく会の画像をディレクトリに置く
追加：シンプルなCSSを追加（スタート地点）
追加：Sassを有効にする
追加：もくもく会のデザインにする
追加：font-awesomeを有効にする
追加：無限ループにする　×
追加：Sassのmixinなどを外だしする

追加：swiperでスライドショー実装


```