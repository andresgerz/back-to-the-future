<template>
  <b-form inline fluid class="form-wrapper">
    <b-col class="my-1" v-for="type in types" :key="type">
      <b-row sm="1">
        <label :for="`type-${type[0]}`">{{ type[1] }}</label>
      </b-row>
      <b-row sm="2">
        <b-form-input :id="`${type[2]}`" :type="`${type[0]}`" :v-model='`${type[2]}`'></b-form-input>
      </b-row>
    </b-col>
  </b-form>
</template>

<script>


export default {
  name: 'form',
  data() {
    return {
      types: [
        ['date', 'Date', 'date'],
        ['number', 'Hour', 'hour'],
        ['number', 'Minute', 'minute']
      ],
      date: '',
      hour: '',
      minuto: ''

    }
  },
  methods: {
    dataDate() {
      this.date;
      this.hour;
      this.minuto;
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