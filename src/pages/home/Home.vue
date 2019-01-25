<template>
    <div>
      <home-header></home-header>
      <home-Swiper></home-Swiper>
    </div>
</template>
<script>
import HomeHeader from "./components/header";
import HomeSwiper from "./components/swiper";
export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper
  }
};
</script>
<style>
</style>

