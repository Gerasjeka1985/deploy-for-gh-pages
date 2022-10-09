<script setup lang="ts">
  import CustomBanner from "~/components/atoms/CustomBanner.vue";
  import Carusel from "~/components/atoms/Carusel.vue";
  import Description from "~/components/atoms/Description.vue";
</script>

<template>
  <div class="content">
    <custom-banner />
    <Carusel />
    <Description />
  </div>
</template>


<style scoped lang="scss">
@import 'assets/scss/_global.scss';


</style>