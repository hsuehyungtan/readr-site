<template>
  <Icon
    :image-path="imagePath"
    :color="color"
    :default-width="defaultWidth"
    :width="width"
    :default-height="defaultHeight"
    :height="height"
  />
</template>

<script>
import Icon from './Icon.vue'

export default {
  components: {
    Icon
  },
  props: {
    color: {
      type: String,
      default: 'white'
    },
    width: {
      type: Number,
      default: null
    },
    height: {
      type: Number,
      default: null
    }
  },
  data () {
    return {
      imagePath: '/public/2.0/icons/series-contents-white.svg',
      defaultWidth: 26,
      defaultHeight: 29
    }
  }
}
</script>

<style lang="stylus" scoped>
</style>
