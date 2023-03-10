<template>
  <swiper :pagination="true" :modules="modules" class="mySwiper testimonial-bg bg-color-overlay">
    <swiper-slide>
      <div class="slider__contents p-5">
        <div class="slider__image">
          <img
            src="https://preview.milingona.co/themes/bakery/catalog/wp-content/uploads/2017/12/testimonial-1-150x150.jpg"
          />
        </div>
        <p class="slider__txt">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. At cupiditate omnis possimus
          illo quos, corporis minima!
        </p>
        <h2 class="slider__caption">Lorem ipsum</h2>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slider__contents p-5">
        <div class="slider__image">
          <img
            src="https://preview.milingona.co/themes/bakery/catalog/wp-content/uploads/2017/12/testimonial-1-150x150.jpg"
          />
        </div>
        <p class="slider__txt">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. At cupiditate omnis possimus
          illo quos, corporis minima!
        </p>
        <h2 class="slider__caption">Lorem ipsum</h2>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slider__contents p-5">
        <div class="slider__image">
          <img
            src="https://preview.milingona.co/themes/bakery/catalog/wp-content/uploads/2017/12/testimonial-1-150x150.jpg"
          />
        </div>
        <p class="slider__txt">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. At cupiditate omnis possimus
          illo quos, corporis minima!
        </p>
        <h2 class="slider__caption">Lorem ipsum</h2>
      </div>
    </swiper-slide>
  </swiper>
</template>
<style scoped>
.bg-color-overlay::before,
.bg-color-overlay::after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1;
}
.bg-color-overlay:before {
  background-color: rgb(114 99 74 / 75%);
}
.testimonial-bg {
  background-image: url('https://images.unsplash.com/photo-1569864358642-9d1684040f43?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1740&q=80');
  background-position: center !important;
  background-repeat: no-repeat !important;
  background-size: cover !important;
}
.slider__contents {
  height: 100%;
  padding: 2rem;
  padding: 5rem;
  text-align: center;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  -ms-flex: 1;
  flex: 1;
  -webkit-flex-flow: column nowrap;
  -ms-flex-flow: column nowrap;
  flex-flow: column nowrap;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: center;
  -webkit-justify-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  z-index: 99;
}
.slider__image {
  margin-bottom: 1rem;
}
.slider__image img {
  border-radius: 30rem;
}
.slider__caption {
  font-weight: 500;
  text-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);
  text-transform: uppercase;
  padding-top: 1rem;
  color: #ffc04c;
}
.slider__caption:before {
  content: '';
  position: absolute;
  width: 30px;
  height: 2px;
  top: 0px;
}

.slider__caption:before {
  background-color: #ccc;
  left: 50%;
  margin-left: -15px;
}

.slider__txt {
  color: #fff;
  margin-bottom: 1rem;
  max-width: 800px;
}
</style>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue'

// Import Swiper styles
import 'swiper/css'

import 'swiper/css/pagination'
// import required modules
import { Pagination } from 'swiper'

export default {
  components: {
    Swiper,
    SwiperSlide
  },
  setup() {
    return {
      modules: [Pagination]
    }
  }
}
</script>
