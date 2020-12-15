<template>
  <div id="app">
    <Display :gYear="getYear" :gMonth="getMonth" :gDay="getDay" :gHour="getHour" :gMin="getMinute" subtitle="DESTINATION TIME" />
    <Display :gYear="getYear" :gMonth="getMonth" :gDay="getDay" :gHour="getHour" :gMin="getMinute" subtitle="PRESENT TIME" />
    <Display :gYear="getYear" :gMonth="getMonth" :gDay="getDay" :gHour="getHour" :gMin="getMinute" subtitle="LAST TIME DEPARTED" />
    <Buttons />
  </div>
</template>

<script>

import Display from './components/Display.vue';
import Buttons from './components/Buttons.vue';

export default {
  name: 'App',
  components: {
    Display,
    Buttons
  },
  methods: {
    getMinute() {
      return new Date().getMinutes();
    },
    getHour() {
      return new Date().getHours();
    },
    getDay() {
      return new Date().getDate();
    },
    getMonth() {
      return String(new Date()).substring(4,7);
    },
    getYear() {
      return new Date().getFullYear(); 
    }
  }
};
</script>

<style>

#app {
  width: 100%;
  background-color: #525358;
  text-align: center;
}


</style>
