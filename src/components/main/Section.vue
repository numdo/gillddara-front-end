<!-- src/components/HeroSection.vue -->
<template>
    <div class="@container">
      <div class="sm:p-4">
        <div
          class="flex min-h-[480px] flex-col gap-6 bg-cover bg-center bg-no-repeat sm:gap-8 sm:rounded-lg items-start justify-end px-4 pb-10 sm:px-10"
          :style="heroStyle"
        >
          <div class="flex flex-col gap-2 text-left">
            <h1
              class="text-white text-4xl font-black leading-tight tracking-tight sm:text-5xl"
            >
              Connect with other passionate travelers
            </h1>
            <h2 class="text-white text-sm font-normal leading-normal sm:text-base">
              Join the Voyage Vista community to share your travel tips and experiences, ask questions, and get advice from fellow adventurers
            </h2>
          </div>
          <button
            class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-lg h-10 px-4 sm:h-12 sm:px-5 bg-green-400 text-gray-900 text-sm font-bold sm:text-base"
          >
            <span class="truncate">Sign up for free</span>
          </button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Section",
    computed: {
      heroStyle() {
        return `background-image: linear-gradient(rgba(0, 0, 0, 0.1) 0%, rgba(0, 0, 0, 0.4) 100%), url("https://cdn.usegalileo.ai/stability/0cba7b67-4ca7-4b5d-b678-cc93c0064a94.png");`;
      },
    },
  };
  </script>
  
  <style scoped>
  .size-full {
    width: 100%;
    height: 100%;
  }
  </style>
  