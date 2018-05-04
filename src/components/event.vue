<template>
  <v-container>
    <v-layout justify-center="true">
      다양한 행사들
    </v-layout>
    <v-layout row>
      <v-flex xs12>
        <v-card class="custom-ripple" ripple style="cursor: pointer;">
          <v-card-media height="500" :src="colors[color]" @click.native="color = (color + 1) % colors.length">
              <v-container fill-height fluid>
              <v-layout fill-height>
                <v-flex xs12 align-end flexbox>
                  <span class="imgHeadline">Top 10 Australian beaches</span>
                </v-flex>
              </v-layout>
            </v-container>
          </v-card-media>
          
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>

</template>

<script>
  import img1 from '../assets/event1.jpg'
  import img2 from '../assets/event2.jpg'
  import img3 from '../assets/event3.jpg'
  import img4 from '../assets/event4.jpg'
  import img5 from '../assets/event5.jpg'
  import img6 from '../assets/event6.jpg'
  import img7 from '../assets/event7.jpg'
  import img8 from '../assets/event8.jpg'
  import img9 from '../assets/event9.jpg'
  import img10 from '../assets/event10.jpg'
  export default {
    data() {
      return {
        color: 0,
        colors: [
          img1, img2, img3, img4, img5, img6, img7, img8, img9, img10
        ]
      }
    }

  }

</script>

<style scoped>
  .custom-ripple {
    user-select: none
  }

  .imgHeadline{
      background-color:rgba(64, 224, 208, 0.7);
      padding:5px;
      border-radius: 3px;
      font : 2.4em bold;
      color:white;
  }

</style>
