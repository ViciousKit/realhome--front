<template>
  <AboutUs />
  <Features :data="featuresData" :color="featuresBgColor"/>
  <OurTeam />
  <Subscribe />
</template>

<script>

import AboutUs from '@/components/About_us.vue';
import Features from '@/components/Features.vue';
import OurTeam from '@/components/OurTeam.vue';
import Subscribe from '@/components/Subscribe.vue';

import {featuresData} from '@/data/data.features.js';

export default {
  name: 'about',
  components: {AboutUs, Features, OurTeam, Subscribe},
  data() {
    return {
      featuresData,
      featuresBgColor: '#f6f6f6'
    }
  }
}
</script>

