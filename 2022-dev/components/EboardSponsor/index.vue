<template>
  <div v-if="sponsorData.sponsor_ad_img" class="eboardSponsor">
    <div class="sponsor__info" :class="{'hasNewsheight': hasNews}">
      <div class="area" style="overflow: hidden;">
        <img :src="sponsorData.sponsor_ad_img" alt="" class="sponsor__img">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EboaedSchedule',
  props: {
    sponsorData: {
      type: Object,
      default: () => {}
    },
    hasNews: {
      type: Boolean,
      default: false
    }
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" src="./style.scss" scoped></style>
