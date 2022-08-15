<template>
  <swiper ref="mySwiper" :options="swiperOptions1" class="slider">
        <swiper-slide class="offer-slide" style="height:400px" >
            <div class="row g-0 h-100">
              <img src="2.jpg" style="max-height:100% max-width:100%" >
            </div>
        </swiper-slide>
            <swiper-slide class="offer-slide" style="height:400px" >
            <div class="row g-0">
              <img src="1.jpg">
            </div>

        </swiper-slide>
        <div class="swiper-button-prev " slot="button-prev"></div>
       <div class="swiper-button-next " slot="button-next"></div>
        <div class="swiper-pagination " slot="pagination"></div>
    </swiper>
</template>

    
<script>
import { Swiper, SwiperSlide, directive } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
   
    components: {
        Swiper,
        SwiperSlide,
    },
    directives: {
        swiper: directive,
    },
    data() {
        return {
            swiperOptions1: {
                slidesPerView: 1,
                freeMode: false,
                loop: false,
                navigation: {
                    nextEl: ".swiper-button-next",
                    prevEl: ".swiper-button-prev",
                },
                autoplay: {
          delay: 1500,
          stopOnLastSlide: false,
          disableOnInteraction: true
        },
                pagination: {
                    el: '.swiper-pagination',
                    type: 'bullets'
                },
            },
            language: '',
            http: 'https://'
        };
    },
    computed: {
        swiper() {
            return this.$refs.mySwiper.$swiper;
        },
    },
 
    mounted() {
        console.log("Current Swiper instance object", this.swiper);
        this.swiper.slideTo(3, 1000, false);
    },
};
</script>
<style scoped>
.slider{
    clip-path: circle(59.7% at 50% 3%);
}
</style>