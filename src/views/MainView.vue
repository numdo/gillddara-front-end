<!-- src/views/MainView.vue -->
<template>
  <div
    class="relative flex w-full min-h-screen flex-col bg-white group/design-root overflow-x-hidden"
    style="font-family: Inter, 'Noto Sans', sans-serif;"
  >
    <div class="flex h-full grow flex-col">
      <!-- 헤더 -->
      <Header />

      <!-- 메인 컨텐츠 -->
      <div class="flex flex-1 justify-center py-5">
        <div class="flex flex-col w-full max-w-7xl">
          <!-- 히어로 섹션 -->
          <Section />

          <!-- 가장 인기 있는 여행지 리스트 -->
          <SpotList />
        </div>
      </div>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from "@/components/common/Header.vue";
import Section from "@/components/main/Section.vue"; // 파일 이름이 Section.vue에서 HeroSection.vue로 변경되었다고 가정
import SpotList from "@/components/common/SpotList.vue"; // 파일 이름이 SpotList.vue에서 TravelSpotList.vue로 변경되었다고 가정
import Footer from '@/components/common/Footer.vue';
export default {
  name: "MainView",
  components: {
    Header,
    Section,
    SpotList,
    Footer,
  },
};
</script>

<style scoped>
/* 필요하지 않은 size-full 클래스 제거 */
</style>
