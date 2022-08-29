<template>
  <div>
    <div class="s-title s4-title">
      <h2 class="h2">STUDENT WORKS</h2>
    </div>
    <div class="s-content s4-content">
      <FormSingle />
    </div>
  </div>
</template>

<script>
import FormSingle from "@/components/FormSingle.vue";

export default {
  components: {
    FormSingle,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.s4-title {
  width: 301px;
  height: 44px;
  left: 50%;
  margin-left: -150.5px;
  position: absolute;
  top: -8%;
  z-index: 1;

  @include min-width(768px) {
    width: 301px;
    height: 44px;
    left: 50%;
    margin-left: -150.5px;
  }

  @include min-width(1025px) {
    top: -8%;
    left: 0;
    margin-left: 0;
  }

  @include min-width(1440px) {
    width: 377.3px;
    height: 55.3px;
    margin-left: 100px;
    top: -12%;
  }

  @include min-width(1920px) {
    width: 539px;
    height: 79px;
    top: -15%;
  }

  .h2 {
    width: 100%;
    height: 100%;
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
    background: url("@/assets/images/pic/pic_07_DREAMON.svg") no-repeat
      center/contain;
    @include hidetext;
  }
}
</style>