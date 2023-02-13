<template>
  <div>
    <home-header></home-header>
    <home-swiper :list="swiperList"></home-swiper>
  </div>
</template>

<script>
import HomeHeader from "./components/Header";
import HomeSwiper from "./components/Swiper";
export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper
  }
};
</script>

<style></style>
