<template>
  <div class="home">
    <Carousel />
    <div class="container">
      <div class="row row_offering">
        <div class="col-md-4 col_one">
          <h3 class="offer_title row_offering_border">We are Offering the Best Estate Deals</h3>
        </div>
        <div class="col-md-8">
          <p class="offer_text">Quisque diam lorem interdum vitaapibus ac scelerisque vitae
          pede. Donec eget tellus non erat lacinia fertum. Donec in velit
          vel ipsum auctovinar. Proin umcorper urna et felisstibulum 
          iaculis lacinia est. Proin dictum elem entum velit fusce euismod. Aenean commodo ligula eget dolor. Aenean massa. Lorem ipsum dolor sit amet, consec tetuer adipis elit, aliquam eget nibh etlibura. Lorem ipsum dolor sitamet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et.
          </p>
        </div>
      </div>
    </div>
    <Features :data="featuresData" :color="featuresBgColor"/>
    <Properties :data="propertiesData"/>
    <HomeSlider />
    <div class="get_started container">
      <div class="row">
        <div class="col-md-7 get_started_text">
          <h1>Get Started on Buying Your <b>New Home</b></h1>
        </div>
        <div class="col-md-2 get_started_button offset-md-3 d-flex justify-content-center align-self-center">
          <button type="button" class="btn btn-primary">MORE ABOUT US</button>
        </div>
        </div>
    </div>
    <Testimonials-slider />
    <Partners />
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from '@/components/Carousel';
import Features from '@/components/Features.vue';
import Properties from '@/components/Properties.vue';
import HomeSlider from '@/components/HomeSlider.vue';
import TestimonialsSlider from '@/components/TestimonialsSlider.vue';
import Partners from '@/components/Partners.vue';

import {featuresData} from '@/data/data.features.js';
import {propertiesData} from '@/data/data.properties.js';


export default {
  name: 'Home',
  components: { 
    Carousel,
    Features,
    Properties,
    HomeSlider,
    TestimonialsSlider,
    Partners,
  },
  data() {
    return {
      featuresData,
      propertiesData,
      featuresBgColor: '#fcfcfc',
    }
  }
}
</script>
