<template>
  <v-container grid-list-lg fluid>
    <v-layout wrap>
      <v-flex xs12 sm9 md7>
        <v-card flat>
          <v-card-media src=img2>
            <img src='../assets/seminar-2.png' alt="">
          </v-card-media>
        </v-card>
      </v-flex>
    </v-layout>
    <v-layout>
    <v-flex offset-xs1 xs5>
      <v-card flat>
        <v-card-text>
          전공과 관련없어도 지원가능합니다.
          <br> 8주차에 걸친 교육으로 실력을 쌓아드립니다.
        </v-card-text>
      </v-card>
    </v-flex>
    <v-flex xs7 id="card2">
        <v-card flat>
          <v-card-media src=img2>
            <img src='../assets/seminar-2.png' alt="">
          </v-card-media>
        </v-card>
      </v-flex>
    
    </v-layout>

  </v-container>
</template>

<script>
  import img1 from '../assets/seminar-1.png'
  import img2 from '../assets/seminar-2.png'
  export default {
    data() {
      return {
        img2: img2
      }
    },
  }
  
</script>

<style scoped>
@media all and (max-width: 950px){
    #card2{
        display:none;
    }
}


</style>
