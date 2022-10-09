<script setup lang="ts">

</script>

<template>
  <div class="banner">
      <p>
        We are
          <strong>
            faster
          </strong>
        <br />
        than sound of wave
      </p>
      <p class="banner__text">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit.
        Aliquam amet asperiores at atque culpa dignissimos eaque eligendi
        eos esse et exercitationem illo, illum incidunt iste magnam maiores
        minima molestiae molestias neque non perspiciatis quae quaerat quod
        quos repellendus sed sequi sint tempora vero voluptate voluptates?
      </p>
  </div>
</template>


<style scoped lang="scss">
@import 'assets/scss/_global.scss';

  .banner{
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 32px;
    width: 100%;
    height: 600px;
    background: url('https://99px.ru/sstorage/53/2015/12/tmb_154087_1126.jpg') center center ;

    &__text{
      display: none;
    }
  }

@include breakpoint(large) {
  .banner {
    justify-content: space-around;
    flex-direction: column;
    background: url('https://99px.ru/sstorage/53/2015/12/tmb_154087_1126.jpg') ;
    background-size: 100% 100%;

    &__text{
      font-size: 16px;
      width: 50%;
      height: 100px;
      display: block;
    }
  }
}

</style>