<script setup lang="ts">

</script>

<template>
  <div class="description">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit.
    Alias atque corporis cupiditate dolor eos itaque magnam molestias
    odit quam, soluta, tempore veritatis voluptates. Architecto eveniet
    explicabo impedit quaerat sed. Eius et facere hic iure maiores nemo
    pariatur perferendis rerum vitae voluptates? Earum illum incidunt quae reiciendis,
    similique tenetur vitae! Alias debitis facere fuga, itaque neque numquam ratione suscipit
    veritatis voluptates. Facilis ipsa laborum molestias sit tempore tenetur, veniam. Architecto assumenda,
    aut dolore earum eligendi fugit magnam officia quibusdam totam vero? A accusamus aut eum,
    facere id incidunt iure labore magni molestias mollitia, nam nulla officia porro sunt tempora,
    velit voluptas voluptatibus!
  </div>
</template>

<style scoped lang="scss">
@import '@/assets/scss/_global.scss';
  .description{
    display: flex;
    justify-content: center;
    align-items: center;
    color: #090979;
  }

@include breakpoint(large) {
  .description{
    width: 600px;
    height: 400px;
    margin: auto;
  }
}
</style>