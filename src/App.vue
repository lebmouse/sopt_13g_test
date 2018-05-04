<template>
  <div id="app">
    <v-app @scroll="op2">
      <!-- <v-app v-scroll="onScroll"> -->
      <!-- <ToolBar v-bind:op="offsetTop"></ToolBar> -->
      <ToolBar :barOption="options" ></ToolBar>
      <v-content>
        <banner id="section1" style="margin-top: 50px;"></banner>
        <introduce></introduce>
        <seminar></seminar>
        <Section2 id="section2"></Section2>
        <Section3 id="section3"></Section3>
        <app-zam></app-zam>
        <event></event>
      </v-content>
      <v-footer dark color="blue"></v-footer>
    </v-app>
  </div>

</template>

<script>
  import ToolBar from './components/toolbar.vue'
  import introduce from './components/introduce.vue'
  import seminar from './components/seminar.vue'
  import Section1 from './components/section1.vue'
  import appzam from './components/appzam.vue'
  import Section2 from './components/section2.vue'
  import Section3 from './components/section3.vue'
  import Section4 from './components/section4.vue'
  import event from './components/event.vue'

  export default {
    components: {
      'ToolBar': ToolBar,
      'banner': Section1,
      'Section2': Section2,
      'Section3': Section3,
      'Section4': Section4,
      introduce, seminar,'app-zam':appzam,event
    },
    data() {
      return {
        options: {
          duration: 685,
          offset: -100,
          easing: 'easeInOutQuad'
        }
      }
    },
    methods: {
      // onScroll(e) {
      //   if (document.documentElement.scrollTop > 150 && this.offsetTop > 0.6) {
      //     this.offsetTop = this.offsetTop - 0.08;
      //   } else if (document.documentElement.scrollTop <= 100) {
      //     this.offsetTop = 1;
      //   }
      // },
      op2() {
        let top = document.documentElement.scrollTop;
        console.log(top);
      }
    }
  }

</script>

<style scoped>


</style>
