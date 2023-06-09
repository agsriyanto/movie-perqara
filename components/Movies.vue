<template>
  <section>
    <div class="bg-[#292e35] absolute h-80 w-full z-0"></div>
    <div class="p-24 pt-16 relative">
      <div class="border-t-[6px] border-[#E74C3C] pt-2 w-24 z-10">
        <label class="font-semibold text-4xl text-[#E5E5E5] whitespace-nowrap">Movies</label>
      </div>
      <div class="pt-14 flex gap-7">
        <div class="bg-[#0f1826] rounded-lg min-w-[240px] h-fit">
          <div class="p-4 text-base font-semibold border-[#292e35] border-b-[1px]">
            <label class="text-white">Sort Result By</label>
          </div>
          <div class="p-4 border-[#292e35] border-b-[1px]">
            <label class="text-white">Popularity</label>
          </div>
          <div class="p-4 text-base font-semibold border-[#292e35] border-b-[1px]">
            <label class="text-white">Genres</label>
          </div>
          <div class="p-4 grid gap-1">
            <Checkbox name="Action" val="Action" v-model="idealfor">Action</Checkbox>
            <Checkbox name="Adventure" val="Adventure" v-model="idealfor">Adventure</Checkbox>
            <Checkbox name="Animation" val="Animation" v-model="idealfor">Animation</Checkbox>
            <Checkbox name="Comedy" val="Comedy" v-model="idealfor">Comedy</Checkbox>
            <Checkbox name="Crime" val="Crime" v-model="idealfor">Crime</Checkbox>
            <Checkbox name="Documentary" val="Documentary" v-model="idealfor">Documentary</Checkbox>
            <Checkbox name="Drama" val="Drama" v-model="idealfor">Drama</Checkbox>
            <Checkbox name="Family" val="Family" v-model="idealfor">Family</Checkbox>
            <Checkbox name="Fantasy" val="Fantasy" v-model="idealfor">Fantasy</Checkbox>
            <Checkbox name="History" val="History" v-model="idealfor">History</Checkbox>
            <Checkbox name="Horror" val="Horror" v-model="idealfor">Horror</Checkbox>
          </div>
        </div>
        <div class="flex flex-wrap gap-7">
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <CardMovies />
          <div class="m-auto pt-[30px]">
            <button class="text-[#E5E5E5] bg-[#FF0000] rounded-[32px] py-1 px-7">Load More</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Checkbox from './Checkbox.vue';
import CardMovies from './CardMovies.vue';

export default 
{
  components: {
    Checkbox,
    CardMovies,
    CardMovies
},
  data() {
    return {
      idealfor: ["movies"]
    }
  }
}
</script>