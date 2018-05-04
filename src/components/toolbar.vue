<template>

  <v-toolbar height="80px" dark fixed color="blue" v-bind:style="{ opacity : op}" @scroll="op2">
    <!-- <v-toolbar height="80px" dark fixed color="blue" v-bind:style="{ opacity : op}" v-on:mouseover="op = 1" @mouseleave="op = 0.4">  -->
    <v-toolbar-title>
      <img src="../assets/22nd_LOGO_white.png" height="55px">
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn flat v-for="{name, id} in btnObj" :key="name" @click="$vuetify.goTo(id,barOption)">{{name}}</v-btn>
    </v-toolbar-items>
  </v-toolbar>


</template>

<script>
  export default {
    props: ['barOption'],
    data() {
      return {
        op: 1,
        btnObj: [{
            name: "One",
            id: "#section1"
          },
          {
            name: "Two",
            id: "#section2"
          },
          {
            name: "Three",
            id: "#section3"
          },
          {
            name: "Four",
            id: "#section4"
          },
          {
            name: "Five",
            id: "#section5"
          }
        ]
      }
    },
    methods: {
      op2() {
        let top = document.documentElement.scrollTop;
        console.log(top);
      }
    },
    computed: {

    }
  }

</script>

<style scoped>


</style>
