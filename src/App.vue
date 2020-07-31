<template>
  <div id="app">
    <Display year="1985" month="OCT" day="26" hour="01" min="21" subtitle="DESTINATION TIME" />
    <Display year="1985" month="OCT" day="26" hour="01" min="22" subtitle="PRESENT TIME" />
    <Display year="1985" month="OCT" day="26" hour="01" min="20" subtitle="LAST TIME DEPARTED" />
  </div>
</template>

<script>

import Display from './components/Display.vue';
import Form from './components/Form.vue';

export default {
  name: 'App',
  components: {
    Display,
    Form
  }

  
}
</script>

<style>

#app {
  width: 100%;
  height: 100vh;
  background-color: #525358;
  text-align: center;
}


</style>
