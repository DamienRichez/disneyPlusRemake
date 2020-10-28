<template>

  <div class="col-md-3 mb-5 cards">
     <img :src="films.img"  class="card-img-top" alt="">
     <h6>{{ films.name }}</h6>
  </div>

</template>

<script>
export default {
    name: 'Cards',
    props: ['films']
}
</script>

<style>

</style>