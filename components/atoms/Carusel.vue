<script setup lang="ts">
import {ref} from 'vue';
  const index = ref(0);
  const arr = [
    {
      img: 'https://sutochno.ru/doc/images/galleries/180/vershina1.jpg'
    },
    {
      img: 'https://www.rgo.ru/sites/default/files/styles/head_image_article/public/node/56828/mariya-shevchenko-kardiogramma-gor-462677-beluha.jpg?itok=X2o_utMw'
    },
    {
      img: 'https://moya-planeta.ru/upload/images/xl/95/fe/95fe44d0e5fe53e49d874f9c2e07381ca8ea823a.jpg'
    },
    {
      img: 'https://bipbap.ru/wp-content/uploads/2017/08/748104.jpg'
    },
    {
      img: 'https://pix-feed.com/wp-content/uploads/2020/05/0-24.jpg'
    },
  ]

  function prev() {
    if(index.value == 0){
      return index.value;
    }
      return index.value--;
  }

  function next() {
    if (index.value == arr.length - 1){
      return index.value;
    }
    return index.value++;
  }

</script>

<template>
  <div class="wrapper">
    <div class="wrapper__carusel">
      <img :src="arr[index].img" alt="image" />
    </div>
  </div>
  <div class="wrapper__btns">
    <button @click.prevent="prev">Prev</button>
    <button @click.prevent="next">Next</button>
  </div>
</template>

<style scoped lang="scss">
@import '@/assets/scss/_global.scss';
  .wrapper{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 300px;

    &__carusel{
      width: 200px;
      height: 200px;

      & img{
        width: 100%;
        height: 100%;
      }
    }

    &__btns{
      width: 100%;
      height: 50px;
      display: flex;
      justify-content: center;
      align-items: center;


      & button {
        cursor: pointer;
        background:$color-primary-blue;
        padding: 7px 10px;
        margin: 10px;
        border-radius: 10px;
        color:$color-primary-white;
      }
    }
  }

  @include breakpoint(large) {
   .wrapper{
     height: 500px;

     &__carusel{
       width: 400px;
       height: 400px;

       & img{
         width: 100%;
         height: 100%;
       }
     }
   }
  }
</style>