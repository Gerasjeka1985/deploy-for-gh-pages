<template>
  <div class="main">
    <h1>Hello world!</h1>
    <h2>Darling Ila its me Jeka ))))</h2>

    <p>click me )))</p>
    <button style="width: 100px;height: 50px;border-radius: 5px" @click="handler">Click</button>
    <div v-if="a">
      <h2>Hi my love ))))</h2>
    </div>
  </div>

</template>

<script setup lang="ts">
import {ref} from 'vue';
  const a = ref(false)
  const handler = () => {
    a.value= true;
  }

</script>

<style scoped>
.main{
  color: aliceblue;
  width: 100%;
  height: 100vh;
  background-image: url("@/assets/images/fdfe5baa-657f-44da-84cb-7f3e4ace13a4_1.jpg");
  background-repeat: no-repeat;
  background-position: center center;
  background-attachment: fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
</style>