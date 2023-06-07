<template>
  <nav class="bg-[#292e35] flex items-center gap-11 justify-center max-h-16">
    <div class="cursor-pointer">
      <img src="../static/MoovieTime-Logo.svg" alt="logo-1" />
    </div>
    <div class="flex items-center gap-4 bg-[#1e232a] p-2 px-4 rounded">
      <img src="../static/icon-mov.svg" alt="logo-2" />
      <input type="text" placeholder="Find movie" class="bg-[#1e232a] w-96" />
      <img src="../static/icon-search.svg" alt="logo-search" class="w-4" />
    </div>
    <div>
      <ul class="flex gap-11">
        <li>
          <div class="flex gap-4 cursor-pointer" id="dropdownNavbarLink" data-dropdown-toggle="dropdownNavbar">
            <img src="../static/icon-category.svg" alt="logo-category" class="w-5" />
            <a class="uppercase text-white">Categories</a>
          </div>
          <div id="dropdownNavbar" class="z-10 hidden font-normal bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700 dark:divide-gray-600">
            <ul class="py-2 text-sm text-gray-700 dark:text-gray-400" aria-labelledby="dropdownLargeButton">
              <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Action</a>
              </li>
              <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Adventure</a>
              </li>
              <li>
                <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Animation</a>
              </li>
            </ul>
        </div>
        </li>
        <li>
          <a class="uppercase text-white cursor-pointer">Movies</a>
        </li>
        <li>
          <a class="uppercase text-white cursor-pointer">TV Shows</a>
        </li>
        <li>
          <a class="uppercase text-white cursor-pointer">LOGIN</a>
        </li>
      </ul>
    </div>
  </nav>
</template>
