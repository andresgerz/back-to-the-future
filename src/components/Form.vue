<template>
  <b-form inline fluid class="form-wrapper">
    <b-col class="my-1" v-for="type in types" :key="type">
      <b-row sm="1">
        <label :for="`type-${type[0]}`">{{ type[1] }}</label>
      </b-row>
      <b-row sm="2">
        <b-form-input :id="`type-${type[0]}`" :type="`${type[0]}`"></b-form-input>
      </b-row>
    </b-col>
  </b-form>
</template>

<script>


export default {
    data() {
      return {
        types: [
          ['date', 'Date'],
          ['number', 'Hour'],
          ['number', 'Minute']
        ]
      }
    }
}
</script>

<style>
  
  .form-wrapper {
    width: 80%;
    margin: auto;
  }

  label {
    width: 50%;
    text-align: center;
  }

</style>