<template>
  <div id="app">
    <h1>Back to the future</h1>

    <Display/>
  </div>
</template>

<script>

import Display from './components/Display.vue';

export default {
  name: 'App',
  components: {
    Display
  }

  
}
</script>

<style>
#app {
  background-color: #525358;
  text-align: center;
}


</style>
