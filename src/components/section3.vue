<template>
  <section class="blue darken-3">
    <v-container grid-list-xs dark>
      <v-layout wrap>
        <v-flex xs12 text-xs-center>
          <h1 class="white--text">8주에 걸친 세미나</h1>
        </v-flex>
        <v-flex offset-sm2 sm8>
          <v-carousel height="600">
            <v-carousel-item >
              <v-card>
                <v-card-media :src="items[0].src" height=600>
                  <v-container fill-height fluid>
                    <v-layout fill-height>
                      <v-flex xs12 align-end flexbox>
                        <span class="headline white--text" v-text="items[0].txt"></span>
                      </v-flex>
                    </v-layout>
                  </v-container>
                </v-card-media>
              </v-card>
            </v-carousel-item>
            <v-carousel-item>
              <img :src="items[1].src" width="100%">
            </v-carousel-item>
            <v-carousel-item height=600>
              <img :src="items[2].src"  width="100%">
            </v-carousel-item>
            <v-carousel-item height=600>
              <img :src="items[3].src"  width="100%">
            </v-carousel-item>
          </v-carousel>
        </v-flex>
      </v-layout>
    </v-container>
  </section>
</template>


<script>
  import img1 from '../assets/section3-1.jpg'
  import img2 from '../assets/section3-2.jpg'
  import img3 from '../assets/section3-3.jpg'
  import img4 from '../assets/section3-4.jpg'
  
  export default {
    data() {
      return {
        items: [{
            src: img1,
            txt: "이것은 첫 번째 이미지"
          },
          {
            src: img2
          },
          {
            src: img3
          },
          {
            src: img4
          }
        ]
      }
    }
  }

</script>

<style>
</style>
