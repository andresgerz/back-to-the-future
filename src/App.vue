<template>
  <div id="app">
    <h1>Back to the future</h1>

    <Display/>
    <Form/>
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
  background-color: #525358;
  text-align: center;
}


</style>
