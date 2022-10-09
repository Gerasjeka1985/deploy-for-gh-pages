<script setup lang="ts">
  import CustomNav from "~/components/atoms/CustomNav.vue";
</script>

<template>
  <div class="header">
      <custom-nav />
  </div>
</template>


<style scoped lang="scss">
@import 'assets/scss/_global.scss';

  .header{
    background: $color-primary-blue;
    background-size: 400% 400%;
    animation: gradient 10s ease infinite;
    transform: translate3d(0, 0, 0);

    @keyframes gradient {
      0% {
        background-position: 0% 50%;
      }
      50% {
        background-position: 100% 50%;
      }
      100% {
        background-position: 0% 50%;
      }
    }
  }
</style>