<template>
  <section class="bg-[#1e232a] min-h-screen">
    <Poster />
    <Review />
    <Recomendation />
  </section>
</template>

<script>
import Poster from '../../components/Poster.vue';
import Review from '../../components/Review.vue';
import Recomendation from '../../components/Recomendation.vue';

export default {
  components: {
    Poster,
    Review,
    Recomendation,
  }
}

</script>