<template>
  <section id="intro">

    <video src="~@/assets/ocean_-_74888 (1080p).mp4" autoplay muted loop></video>
    <!-- <div class="new_pjt">
      <p>PROJECT!</p>
      <swiper
      :slidesPerView="2"
      :centeredSlides="true"
      :spaceBetween="30"
      :pagination="{
        clickable: true,
      }"
      :modules="modules"
      class="mySwiper"
      >
        <swiper-slide>Slide 1</swiper-slide>
        <swiper-slide>Slide 2</swiper-slide><swiper-slide>Slide 3</swiper-slide>
        <swiper-slide>Slide 4</swiper-slide><swiper-slide>Slide 5</swiper-slide>
        <swiper-slide>Slide 6</swiper-slide><swiper-slide>Slide 7</swiper-slide>
        <swiper-slide>Slide 8</swiper-slide><swiper-slide>Slide 9</swiper-slide>
      </swiper>
    </div> -->
  </section>
</template>


<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import { Pagination } from 'swiper/modules';


</script>

<style lang="less" scoped>
#intro {
  width: 100%;
  // display: flex;
  // justify-content: center;
  
}
</style>
