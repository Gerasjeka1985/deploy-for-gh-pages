<script setup lang="ts">
  import CustomHeader from "~/components/organism/CustomHeader.vue";
  import CustomFooter from "~/components/organism/CustomFooter.vue";
  import Content from "~/components/organism/Content.vue";
</script>

<template>
  <div class="main">
    <custom-header class="main__header" />
    <Content />
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
}
</style>