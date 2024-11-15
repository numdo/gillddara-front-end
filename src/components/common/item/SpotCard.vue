<!-- src/components/SpotCard.vue -->
<template>
    <div class="flex flex-col gap-3 pb-3">
      <div
        class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-lg"
        :style="`background-image: url('${imageUrl}');`"
      ></div>
      <div>
        <p class="text-gray-900 text-base font-medium">{{ title }}</p>
        <p class="text-neutral-500 text-sm font-normal">{{ location }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "SpotCard",
    props: {
      imageUrl: {
        type: String,
        required: true,
      },
      title: {
        type: String,
        required: true,
      },
      location: {
        type: String,
        required: true,
      },
    },
  };
  </script>
  
  <style scoped>
  /* 추가 스타일이 필요하면 여기에 작성 */
  </style>
  