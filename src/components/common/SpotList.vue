<!-- src/components/SpotList.vue -->
<template>
    <div>
      <h2 class="text-gray-900 text-[22px] font-bold leading-tight tracking-tight px-4 pb-3 pt-5">
        Most Liked Travel Spots
      </h2>
      <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
        <SpotCard
          v-for="(spot, index) in travelSpots"
          :key="index"
          :imageUrl="spot.imageUrl"
          :title="spot.title"
          :location="spot.location"
        />
      </div>
    </div>
  </template>
  
  <script>
  import SpotCard from "@/components/common/item/SpotCard.vue";
  
  export default {
    name: "SpotList",
    components: {
      SpotCard,
    },
    data() {
      return {
        travelSpots: [
          {
            imageUrl: "https://cdn.usegalileo.ai/sdxl10/6c26b46c-592e-4b6b-9b09-f68c69f6df8f.png",
            title: "Bora Bora",
            location: "French Polynesia",
          },
          {
            imageUrl: "https://cdn.usegalileo.ai/stability/78f4e159-178f-45b1-9ab0-5597bd48e8e2.png",
            title: "Santorini",
            location: "Greece",
          },
          {
            imageUrl: "https://cdn.usegalileo.ai/stability/897fe2c1-7397-436a-8906-3d270fa53352.png",
            title: "Kyoto",
            location: "Japan",
          },
          {
            imageUrl: "https://cdn.usegalileo.ai/stability/4ac71f43-4b1b-442b-a044-d82a8b3a58ce.png",
            title: "Maui",
            location: "Hawaii",
          },
          // 추가적인 여행지 정보를 여기에 추가할 수 있습니다.
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* 추가 스타일이 필요하면 여기에 작성 */
  </style>
  