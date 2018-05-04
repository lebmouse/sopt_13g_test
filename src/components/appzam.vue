<template>
  <section id="appzamSection">
    <div class="zamLayout">
      <div class="zamCard">
        <div class="cardCover1">
          커버첫번째
        </div>
        <div class="cardCover2">
          카드커버2
        </div>
        <div class="cardImg">
          <img src="../assets/appzam-re3.png">
        </div>
      </div>
      <div class="zamCard">
        <div class="cardCover1">
          이건 두번쨰
        </div>
        <div class="cardCover2">
          카드커버2
        </div>
        <div class="cardImg">
          <img src="../assets/appzam-re1.png">
        </div>
      </div>
      <div class="zamCard">
        <div class="cardCover1">
          이건 두번쨰
        </div>
        <div class="cardCover2">
          카드커버2
        </div>
        <div class="cardImg">
          <img src="../assets/appzam-re4.png">
        </div>
      </div>
    </div>
  </section>

</template>

<script>
  import appzam1 from '../assets/appzam-re1.png'
  export default {
    data() {
      return {
        // img1 : appzam1
      }
    },
    methods: {
      overTrans(e) {
        // e.target.innerText = '이건 트랜스문자이다.';
      },
      outTrans(e) {
        // e.target.innerText = '이건 글자이다.';
      }
    }

  }

</script>

<style scoped>
  .zamLayout {
    display: flex;
    justify-content: center;
  }

  .zamCard {
    float: left;
  }

  .zamCard>.cardCover1 {
    background-color: rgba(135, 206, 250, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 667px;
    width: 333px;
    position: absolute;
    content: "CSS";
    opacity: 1;
    color:white;
    font: 3em bold;
  }

  .zamCard:hover>.cardCover1 {
    animation: coverTrans1 0.75s;
    opacity: 0;
  }

  @keyframes coverTrans1 {
    0% {
      opacity: 1;
    }
    75% {
      opacity: 0;
    }
  }

  .zamCard>.cardCover2 {
    background-color: rgba(135, 206, 250, 0.6);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 667px;
    width: 333px;
    position: absolute;
    content: "CSS";
    opacity: 0;
    color:white;
    font: 2.5em bold;
  }

  .zamCard:hover>.cardCover2 {
    animation: coverTrans2 0.75s;
    opacity: 1;
  }

  @keyframes coverTrans2 {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

</style>
