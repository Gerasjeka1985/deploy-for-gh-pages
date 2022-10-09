<script setup lang="ts">
  import CustomHeader from "~/components/organism/CustomHeader.vue";
  import CustomFooter from "~/components/organism/CustomFooter.vue";
</script>

<template>
  <div class="main">
    <custom-header class="main__header" />
    <custom-footer class="main__footer" />
  </div>
</template>

<style scoped lang="scss">
@import '@/assets/scss/_global.scss';
.main{
  position: relative;
  width: 100%;
  min-height: 100vh;
  background: $color-primary-gray;
  color: $color-primary-white;

  &__footer{
    position: absolute;
    bottom: 0;
  }
}
</style>