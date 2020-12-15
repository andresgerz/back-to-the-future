<template>
  <div class="container w-50 bg-primary">
    <div class="container w-50 d-flex flex-column">
      <div>led</div>
      <div>led</div>
      <div>led</div>
      <div>led</div>
      <div>led</div>
    </div>
    <form class="container buttons-wrapper">
      <div class="d-flex flex-wrap">
        <button>1</button>
        <button>2</button>
        <button>3</button>
        <button>4</button>
        <button>5</button>
        <button>6</button>
        <button>7</button>
        <button>8</button>
        <button>9</button>
        <button>0</button>
      </div>
    </form>    
  </div>
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
  
  .buttons-wrapper {
    width: 120px;
  }

  label {
    width: 50%;
    text-align: center;
  }

</style>