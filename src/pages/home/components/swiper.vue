<template>
    <div  class="wrapper">
    <swiper :options="swiperOption">
        <!-- slides -->
        <swiper-slide v-for='itme of swiperList' :key="itme.id"><img class="home-swiper" :src="itme.imgUrl"></swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
    </div> 
</template>
<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
        pagination: ".swiper-pagination",
        loop:'true'
      },
      swiperList: [
        {
          id: "01",
          imgUrl:
            "https://source.qunarzz.com/site/images/wns/20181227_qunar_homepage_dujia_5.jpg"
        },
        {
          id: "02",
          imgUrl:
            "https://source.qunarzz.com/site/images/wns/20190119_dujia_homepage_top_banner_1.jpg"
        }
      ]
    };
  }
};
</script>
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active {
    background-color: #fff;
}

.wrapper {
    width: 100%;
    height: 0;
    overflow: hidden;
    padding-bottom: 31.25%;

    .home-swiper {
        width: 100%;
    }
}
</style>

