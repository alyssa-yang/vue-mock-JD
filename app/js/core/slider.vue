

<template lang="html">
    <section :class="cname">
        <swiper :options="options" ref="mySwiper" >
            <swiper-slide v-for="item in items" :key="item.href">
                <router-link :to="{name:item.href}">
                    <img :src="item.src">
                </router-link>
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
            <!-- <div class="swiper-pagination" v-if="options.pagination" slot="pagination"/> -->
        </swiper>
    </section>
</template>


<script>
import { swiper, swiperSlide } from "vue-awesome-swiper";

export default {
  name: "carrousel",
  components: {
    swiper,
    swiperSlide
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.swiper;
    }
  },
  mounted() {
    this.swiper.slideTo(3, 1000, false);
  },
  props: {
    cname: {
      type: String,
      default: ""
    },
    options: {
      type: Object,
      default() {
        return {
          autopay: true,
          loop: true,
          pagination: {
            el: ".swiper-pagination"
          },
          notNextTick: false
        };
      }
    },
    items: {
      type: Array,
      default() {
        return [];
      }
    }
  }
};
</script>


<style lang="css">
@import "~swiper/dist/css/swiper.css";
</style>
