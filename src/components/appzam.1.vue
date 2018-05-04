<template>
  <section id="appzamSection">
    <!-- <div class="imgCard">
    </div> -->
    <div class="appzamCard card1">

      <img src="../assets/appzam1.jpg">

    </div>
    <div class="appzamCard card2">
      <img src="../assets/appzam2.jpg">
    </div>
    <div class="appzamCard card3">
      <img src="../assets/appzam3.jpg">
    </div>
  </section>

</template>

<script>
  export default {

  }

</script>

<style scoped>
  #appzamSection {}

  .appzamCard {
    /* display: block; */
    float: left;
    height: 667px;
    width: 33.33%;
    z-index: 1;
    position: absolute;
    text-align: center;
  }

  #appzamSection img {
    height: 100%;
    z-index: 1;
    /* position: absolute; */
  }

  .imgCard {
    background-color: rgba(255, 0, 0, 0.37);
    height: 667px;
    width: 100%;
    position: absolute;
    z-index: 3;
  }

  .card1 {
    background-color: red;
  }

  .card1:hover {
    background-color: rgba(255, 0, 0, 0.795);
    animation: hoverWidth1;
    animation-duration: 1.5s;
    width: 100%;
    z-index: 2;

  }

  .card2 {
    background-color: blue;
    margin-left: 33.33%;
  }

  .card2:hover {
    background-color: rgba(0, 0, 255, 0.788);
    animation: hoverWidth2;
    animation-duration: 1.5s;
    width: 100%;
    margin-left: 0%;
    z-index: 2;
  }

  .card3 {
    background-color: orange;
    margin-left: 66.66%;
  }

  .card3:hover {
    background-color: rgba(255, 166, 0, 0.788);
    animation: hoverWidth3;
    animation-duration: 1.5s;
    width: 100%;
    margin-left: 0%;
    z-index: 2;
  }

  @keyframes hoverWidth1 {
    0% {
      width: 33.33%;

    }
    100% {
      width: 99%;

    }
  }

  @keyframes hoverWidth2 {
    0% {
      width: 33.33%;
      margin-left: 33.33%;
    }
    100% {
      width: 100%;
      margin-left: 0%;
    }
  }

  @keyframes hoverWidth3 {
    0% {
      width: 33.33%;
      margin-left: 66.66%;
    }
    100% {
      width: 100%;
      margin-left: 0%;
    }
  }

</style>
