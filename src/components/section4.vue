<template>
  <v-container grid-list-xs>
    <v-layout row wrap>
      <v-flex xs6 md3>
        <div class="hoverColor">
          <p class="txtHover">이건 마우스가 위에 있으면 보인다.</p>
          <!-- <v-card ripple height="300" style="opacity:0.5" :img='items[1].src' v-on:mouseleave="change">
          </v-card> -->
        </div>
      </v-flex>
      <v-flex xs6 md3>
        <div class="hoverChange">
          <img :src='items[0].src' height="100%" width="100%" alt="">
        </div>
      </v-flex>
      <v-flex xs6 md3>
        <v-card ripple height="300" color="orange">
        </v-card>
      </v-flex>
      <v-flex xs6 md3>
        <v-card ripple tile height="300" color="blue-grey">
        </v-card>
      </v-flex>
    </v-layout>

  </v-container>
</template>

<script>
  import img1 from '../assets/22nd_LOGO_black.png'
  import img2 from '../assets/section4-1.png'
  export default {
    data() {
      return {
        cnt: true,
        items: [{
            src: img1,
          },
          {
            src: img2
          }
        ]
      }
    },
    methods: {
      change() {
        this.cnt = !this.cnt;
        console.log('나 여기 어둠속에 있다.');
        console.log(this.cnt);
      }
    }
  }

</script>

<style scoped>
  .hoverChange {
    background-color: blue;
    height: 300px;
  }

  .hoverChange::after :hover {
    /* transition-duration: 0.5s; */
    background-color: red;
    content: url('../assets/section4-1.png');
    transition: all .3s ease;
    content: "이건 변경된 문자이다."
  }

  .hoverColor {
    /* transition-duration: 0.5s; */
    /* content: url('../assets/section4-1.png'); */
    height: 300px;
  }

  .hoverColor:hover {
    /* transition-duration: 0.5s; */
    background-color: red;
    opacity: 0.8;
    transition: all .3s ease;
  }

</style>
