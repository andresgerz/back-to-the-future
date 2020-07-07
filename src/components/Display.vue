<template>
  <div>
    <div class="container">
      <div class="item">
        <strong>MONTH</strong>
        <p>oct</p>
      </div>
      <div class="item">
        <strong>DAY</strong>
        <p>26</p>
      </div>
      <div class="item">
        <strong>YEAR</strong>
        <p>1985</p>
      </div>
      <div class="item">
        <strong>HOUR</strong>
        <p>01</p>
      </div>
      <div class="item">
        <strong>MIN</strong>
        <p>21</p>
      </div>
    </div>
    <div class="container">
      <div class="item">
        <strong>MONTH</strong>
        <p>oct</p>
      </div>
      <div class="item">
        <strong>DAY</strong>
        <p>26</p>
      </div>
      <div class="item">
        <strong>YEAR</strong>
        <p>1985</p>
      </div>
      <div class="item">
        <strong>HOUR</strong>
        <p>01</p>
      </div>
      <div class="item">
        <strong>MIN</strong>
        <p>22</p>
      </div>
    </div>
    <div class="container">
      <div class="item">
        <strong>MONTH</strong>
        <p>oct</p>
      </div>
      <div class="item">
        <strong>DAY</strong>
        <p>26</p>
      </div>
      <div class="item">
        <strong>YEAR</strong>
        <p>1985</p>
      </div>
      <div class="item">
        <strong>HOUR</strong>
        <p>01</p>
      </div>
      <div class="item">
        <strong>MIN</strong>
        <p>20</p>
      </div>
    </div>
  </div>
</template>


<script>
  export default {

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


  .item p {
    background-color: #000;
    font-size: 64px;
    margin: 0;
  }


  .item strong {
    background-color: #460f0c;
    color: #fff;
    font-size: 22px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    padding: 0 20px;
  }


  .container:first-child {
    color: #fa6a41;
  }


  .container:nth-child(2) {
    color: #7fd757;
  }


  .container.container:nth-child(3) {
    color: #e3b150;
  }

</style>