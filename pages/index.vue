<template>
  <h1>Hello world!</h1>
  <h2>Darling Ila its me Jeka ))))</h2>

  <p>click me )))</p>
  <button style="width: 100px;height: 50px;border-radius: 5px" @click="handler">Click</button>
</template>

<script setup lang="ts">
  const handler = () => {
    alert('kiss you darling ))))')
  }

</script>