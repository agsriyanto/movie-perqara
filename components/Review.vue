<template>
  <section class="bg-white min-h-[540px]">
    <div class="grid absolute left-[23.5%] w-[500px] gap-1 py-6">
      <label class="text-[#FF0000] font-semibold text-sm">OVERVIEW</label>
      <lavel class="text-black text-sm">
        Wonder Woman comes into conflict with the Soviet Union during the Cold War in the 1980s and finds a formidable foe by the name of the Cheetah.
      </lavel>
    </div>
    <div class="p-24 pb-20 pt-[150px]">
      <label class="text-[#FF0000] font-semibold text-sm">REVIEWS</label>
      <div class="flex gap-8 pt-6">
        <CardReview />
        <CardReview />
        <!-- <div class="bg-[#F9F9F9] p-6 rounded-[14px] items-center w-1/2">
          <div class="flex justify-between items-center pb-4">
            <div class="flex items-center">
              <img
                src="https://www.macmillandictionary.com/external/slideshow/thumb/Grey_thumb.png"
                alt="avatar"
                class="w-11 h-11 rounded-full"
              />
              <div class="flex flex-col pl-4">
                <label class="text-sm font-bold text-[#1E232A]">SWITCH.</label>
                <label class="text-xs text-[#666666]">December 18, 2020</label>
              </div>
            </div>
            <div class="bg-[#C4C4C4] flex w-fit p-3 rounded-[7px] items-start">
              <img src="../static/Star 1.svg" alt="start" class="w-6 pt-1 pr-2" />
              <label class="font-semibold text-4xl text-black">7.0</label>
            </div>
          </div>
          <label class="italic text-sm">
            It isn't as easy as saying 'Wonder Woman 1984' is a good or bad movie. The pieces are there, and there are moments I adore, but it does come across as a bit of a mess, even though the action sequences are breathtaking. If you're a fan of the original film, you'll be more willing to take the ride, but for those more indifferent, it may be a bit of a blander sit. If you can and are planning to watch it, the theatrical experience is the way to go - there is nothing like seeing these stunning sets, fun action scenes and hearing Zimmer's jaw-dropping score like on the big screen. - Chris dos Santos...<span class="text-[#E74C3C]"> read the rest.</span>
          </label>
        </div> -->

        <!-- <div class="bg-[#F9F9F9] p-6 rounded-[14px] items-center w-1/2">
          <div class="flex items-center">
            <img
              src="https://www.macmillandictionary.com/external/slideshow/thumb/Grey_thumb.png"
              alt="avatar"
              class="w-11 h-11 rounded-full"
            />
            <div class="flex flex-col pl-4">
              <label class="text-sm font-bold text-[#1E232A]">SWITCH.</label>
              <label class="text-xs text-[#666666]">December 18, 2020</label>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </section>
</template>

<script>
import CardReview from './CardReview.vue';

export default {
  components: {
    CardReview,
  }
}

</script>