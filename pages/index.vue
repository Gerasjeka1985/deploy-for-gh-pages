<template>
  <h1>Hello world!</h1>
  <h2>Darling Ila its me Jeka ))))</h2>

  <p>click me )))</p>
  <button style="width: 100px;height: 50px;border-radius: 5px" @click="handler">Click</button>
  <div v-if="a">
    <h2>Hi my love ))))</h2>
  </div>
</template>

<script setup lang="ts">
import {ref} from 'vue';
  const a = ref(false)
  const handler = () => {
    a.value= true;
  }

</script>