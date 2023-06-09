<template>
  <section class="px-24 py-14">
    <label class="text-sm font-semibold text-white">RECOMMENDATION MOVIES</label>
    <div class="flex flex-wrap gap-8 pt-8 pb-28">
      <CardMovies />
      <CardMovies />
      <CardMovies />
      <CardMovies />
      <CardMovies />
    </div>
  </section>
</template>

<script>
import CardMovies from './CardMovies.vue';

export default {
  components: {
    CardMovies,
  }
}

</script>