<!-- src/components/Header.vue -->
<template>
    <header class="flex items-center justify-between whitespace-nowrap border-b border-solid border-b-gray-200 px-10 py-3">
      <div class="flex items-center gap-4 text-gray-900">
        <div class="size-4">
          <svg
            viewBox="0 0 48 48"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="w-6 h-6"
          >
            <path
              d="M24 4C25.7818 14.2173 33.7827 22.2182 44 24C33.7827 25.7818 25.7818 33.7827 24 44C22.2182 33.7827 14.2173 25.7818 4 24C14.2173 22.2182 22.2182 14.2173 24 4Z"
              fill="currentColor"
            ></path>
          </svg>
        </div>
        <h2 class="text-lg font-bold leading-tight tracking-tight">Voyage Vista</h2>
      </div>
      <div class="flex flex-1 justify-end gap-8">
        <nav class="flex items-center gap-9">
          <a class="text-gray-900 text-sm font-medium" href="#">Travel</a>
          <a class="text-gray-900 text-sm font-medium" href="#">Explore</a>
          <a class="text-gray-900 text-sm font-medium" href="#">Flights</a>
          <a class="text-gray-900 text-sm font-medium" href="#">Hotels</a>
        </nav>
        <button
          class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-lg h-10 px-4 bg-gray-200 text-gray-900 text-sm font-bold"
        >
          <span class="truncate">List</span>
        </button>
        <div
          class="bg-center bg-no-repeat aspect-square bg-cover rounded-full size-10"
          style='background-image: url("https://cdn.usegalileo.ai/stability/c307b912-ecd8-4b9d-9060-115adc028f8f.png");'
        ></div>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: "Header",
  };
  </script>
  
  <style scoped>
  .size-4 {
    width: 1rem; /* 16px */
    height: 1rem; /* 16px */
  }
  
  .size-10 {
    width: 2.5rem; /* 40px */
    height: 2.5rem; /* 40px */
  }
  </style>
  