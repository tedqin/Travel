<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1602/68/68aa05adb5315f9990.water.jpg_600x330_0dcecae1.jpg">
      <div class="banner-info">
        <div class="banner-title">
          北京海洋馆(AAAA景区)
        </div>
        <div class="banner-number">
          <span class="iconfont banner-icon">&#xe674;</span>
          30
        </div>
      </div>
    </div>
    <common-gallery
      :imgs="imgs"
      v-show="showGallery"
      @close="handleGalleryClose"
    ></common-gallery>
 </div>
</template>

<script>
import CommonGallery from 'common/gallery/Gallery'
export default {
  name: 'DetailBanner',
  data () {
    return {
      showGallery: false,
      imgs: ['//img1.qunarzz.com/sight/p0/1602/68/68aa05adb5315f9990.water.jpg_600x330_0dcecae1.jpg', 'http://img1.qunarzz.com/sight/p0/1611/8c/8c31ff91d910f6ada3.img.jpg_r_800x800_5fcc807f.jpg']
    }
  },
  methods: {
    handleBannerClick () {
      this.showGallery = true
    },
    handleGalleryClose () {
      this.showGallery = false
    }
  },
  components: {
    CommonGallery
  }
}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      height: .6rem
      color: #fff
      background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, .8))
      .banner-title
        font-size: .32rem
        padding: 0 .2rem
        flex: 1
      .banner-number
        padding: 0 .4rem
        line-height: .32rem
        height: .32rem
        border-radius: .2rem
        background: rgba(0, 0, 0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
