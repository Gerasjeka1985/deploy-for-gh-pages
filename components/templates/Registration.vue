<script setup lang="ts">
import CustomHeader from "~/components/organism/CustomHeader.vue";
import CustomFooter from "~/components/organism/CustomFooter.vue";
</script>

<template>
  <div class="registration">
    <custom-header class="registration__header" />
    <h2>registration Page</h2>
    <nuxt-link to="/">back to main</nuxt-link>
    <custom-footer class="registration__footer" />
  </div>
</template>

<style scoped lang="scss">
@import '@/assets/scss/_global.scss';

.registration{
  position: relative;
  width: 100%;
  height: 100vh;
  background: $color-primary-gray;
  color: $color-primary-white;

  &__footer{
    position: absolute;
    bottom: 0;
  }
}
</style>