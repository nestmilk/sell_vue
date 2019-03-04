<template>
  <div class="titleA">
    <div class="line"></div>
    <div class="text">{{name}}</div>
    <div class="line"></div>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  name: 'titleA',
  props: {
    titleName: {
      type: String
    }
  },
  data () {
    return {
      name: this.titleName
    }
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .titleA
    display: flex
    width: 80%
    margin: 28px auto 24px auto
    .line
      flex: 1
      position: relative
      top: -6px
      border-bottom: 1px solid rgba(255, 255, 255, 0.2)
    .text
      padding: 0 12px
      font-weight: 700
      font-szie: 14px
</style>
