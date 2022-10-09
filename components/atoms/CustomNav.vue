<script setup lang="ts">
  const links = [
    {
      name: "Main",
      ref: "/"
    },
    {
      name: "about",
      ref: "/about"
    },
    {
      name: "Registration",
      ref: "/registration"
    }
  ]
</script>

<template>
  <div class="nav">
    <div class="nav__logo">
      <img src="https://cdn-icons-png.flaticon.com/512/683/683165.png" alt="icon" />
    </div>
    <ul class="nav__list">
      <li class="nav__item" v-for="link in links">
        <nuxt-link class="nav__link" :to="link.ref">{{link.name}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
  @import '@/assets/scss/_global.scss';

  .nav{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 75px;

    &__logo{
      position: absolute;
      left: 10px;
      top: 13px;
      width: 50px;
      height: 50px;
      background: $color-primary-gray;
      border-radius: 35px;
      & img{
        width: 100%;
        height: 100%;
      }
    }

    &__list{
      width: 220px;
      height: 25px;
      display: flex;
      justify-content: space-around;
      align-items: center;
    }

    &__item {
      list-style-type: none;
    }

    &__link{
      color: white;
      text-decoration: none;
    }
  }

  @include breakpoint(large) {
    .nav {
      &__list {
        width: 550px;
      }
    }
  }
</style>