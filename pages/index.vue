<template>
  <section class="container bg-[#1e232a]">
    <CardCarousel class="py-10 flex justify-center" />
    <Content />
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue';
import Navbar from '../components/Navbar.vue';
import Content from '../components/Content.vue';
import Footer from '../components/Footer.vue';
import CardCarousel from '../components/CardCarousel.vue';
import axios from 'axios';

export default {
  components: {
    AppLogo,
    Navbar,
    Content,
    Footer,
    CardCarousel,
  },
  env: {
    apiKey: process.env.API_KEY,
  },
  data() {
    return {
      options: {
        slidesPerView: 3,
        loop: true,
        pagination: {
          el: '.swiper-pagination'
        }
      }
    }
  },
  async mounted() {
    try {
      const config = {
        headers: {
          'Authorization': `Bearer ${process.env.apiKey}`,
        },
      };
      const response = await axios.get('https://api.themoviedb.org/3/movie/11', config);
      const data = response.data;
      console.log(data);
    } catch (error) {
      console.error(error);
    }
  },
}


// const config = { headers: { 'Authorization': `Bearer 60967d59ebd299b1cbe2f62c06fb1f30` } };
// const { data } = await useFetch('https://api.themoviedb.org/3/movie/11', config)
// console.log({data})
</script>

<style>
.container {
  min-height: 100vh;
  min-width: 100%;
  display: flex;
  flex-direction: column;
  /* justify-content: center; */
  /* align-items: center; */
  /* text-align: center; */
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

