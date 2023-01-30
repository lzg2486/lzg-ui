<template>
 <div class="l-card" :style="width? {width: width + 'px'} : {}">
  <div class="l-card-img" :style="imgHeight ? {height: imgHeight + 'px'} : {}">
    <img :src="imgSrc" alt="img">
  </div>
  <div v-if="summary" class="l-card-summary">
    {{ summary }}
  </div>
  <div v-else class="l-card-summary">
    <slot></slot>
  </div>
  <slot name="footer"></slot>
 </div>
</template>

<script>
export default {
  name: 'l-card',
  props: {
    width: {
      type: Number,
      default: 0
    },
    imgSrc: {
      type: String,
      default:''
    },
    imgHeight: {
      type: Number,
      default:0
    },
    summary: {
      type: String,
      default: ''
    }
  }
}
</script>
<style lang="scss">
@import './card.scss'
</style>