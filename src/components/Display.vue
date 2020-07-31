<template>
  <div id="display">
    <div class="container">
      <div class="item">
        <strong>MONTH</strong>
        <p class="text-time">{{ month }}</p>
      </div>
      <div class="item">
        <strong>DAY</strong>
        <p class="text-time">{{ day }}</p>
      </div>
      <div class="item">
        <strong>YEAR</strong>
        <p class="text-time">{{ year }}</p>
      </div>
      <div class="item am-pm">
        <div><strong>AM</strong></div>
        <div><strong>PM</strong></div>
      </div>
      <div class="item">
        <strong>HOUR</strong>
        <p class="text-time">{{ hour }}</p>
      </div>
      <div class="points">
        <p>.</p>
        <p>.</p>
      </div>
      <div class="item">
        <strong>MIN</strong>
        <p class="text-time">{{ min }}</p>
      </div>
    </div>
    <div class="subtitle">
      <h3 class="text-time"><strong>{{ subtitle }}</strong></h3>
    </div>
  </div>
</template>


<script>
  export default {
    name: 'Display',
    props: {
      month: {
        type: String,
        required: true
      },
      day: {
        type: String,
        required: true
      },
      year: {
        type: String,
        required: true
      },
      hour: {
        type: String,
        required: true
      },
      min: {
        type: String,
        required: true
      },
      subtitle: {
        type: String,
        required: true
      }
    }
  }
</script>


<style media="screen">

  .container {
    height: 150px;
    display: flex;
    justify-content: space-around;
    font-family: 'DSEG7-Classic';
  }
  
  
  .item:first-child p {
    font-family: 'DSEG14-Classic';
  }


  .item .text-time {
    background-color: #000;
    font-size: 64px;
    margin: 0;
  }


  .item strong {
    background-color: #4D0E0D;
    color: #fff;
    font-size: 22px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    padding: 0 20px;
  }


  .subtitle {
    width: 100%;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    color: #fff;
    background-color: #000;
  }


  #display:first-child .container {
    color: #fa6a41;
  }


  #display:nth-child(2) .container {
    color: #7fd757;
  }


  #display:nth-child(3) .container {
    color: #e3b150;
  }


  .points {
    width: 20px;
    font-size: 80px;
  }


  .points p {
    height: 25px;
    margin-top: -20px;
  }

  .am-pm{
    margin-top: 25px;
  }

</style>