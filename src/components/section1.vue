<template>
  <section>
    <v-jumbotron :src=src dark>
      <v-container fill-height>
        <v-layout align-center>
          <v-flex text-xs-center>
            <h3 class="display-3"></h3>
          </v-flex>
        </v-layout>
      </v-container>
    </v-jumbotron>
  </section>
</template>

<script>
import img1 from '../assets/홈페이지소개배너11-1280x350.png'
  export default {
    data(){
      return{
        src : img1
      }
    }
  }

</script>

<style scope>


</style>
