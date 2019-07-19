<template>
  <div class="search">
    <input class="search-input" type="text" placeholder="输入城市名或拼音" />
  </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .search
    padding: 0 .1rem
    height: .72rem
    background: $bgColor
    .search-input
      height: .62rem
      width: 100%
      line-height: .62rem
      text-align: center
      border-radius: .06rem
      color: #666
      padding: 0 .1rem
      box-sizing: border-box
</style>
