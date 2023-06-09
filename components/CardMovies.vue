<template>
  <section class="grid w-fit">
    <div class="group/item cursor-pointer w-fit">
      <div class="w-fit bg-[#292e35] py-1 px-3 font-bold text-lg absolute left-[12.2%]">
        <label class="text-[#E5E5E5]">7.0</label>
      </div>
      <div class="w-56 h-80">
        <img 
          src="https://assets.kompasiana.com/items/album/2016/05/31/145941435073163-800x1143-574d80e57993731408c4959d.jpg?t=o&v=400"
          alt="image"
          class="w-56 h-80 z-0"
        />
        <a class="w-56 h-80 bg-[#292e35] absolute top-auto cursor-default flex content-center items-center text-center justify-center invisible z-10 group-hover/item:visible ...">
          <div class="grid gap-9">
            <div class="flex items-center gap-3">
              <img src="../static/Star 1.svg" alt="start" />
              <label class="text-[#E5E5E5] font-semibold text-2xl">7.0</label>
            </div>
            <label class="text-[#E5E5E5] font-semibold text-lg">Action</label>
            <button class="bg-[#FF0000] text-[#E5E5E5] py-1 px-4 rounded-[32px] text-sm font-semibold">
              <NuxtLink :to="'/detail/123'">
                VIEW
              </NuxtLink>
            </button>
          </div>
        </a>
      </div>
    </div>
    <label class="text-[#E5E5E5] font-semibold text-base pt-2">My Stupid Boss</label>
    <label class="text-[#929292] text-sm">2016</label>
  </section>
</template>