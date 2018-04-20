<template>
  <div id="app">
  <v-app>
    <ToolBar></ToolBar>
    <v-content>
      <Section1></Section1>
      <Section2></Section2>
      <Section3></Section3>
    </v-content>

  </v-app>
  </div>

</template>

<script>
import ToolBar from './components/toolbar.vue'
import Section1 from './components/section1.vue'
import Section2 from './components/section2.vue'
import Section3 from './components/section3.vue'
import Section4 from './components/section4.vue'

export default {
  components:{
    'ToolBar' : ToolBar,
    'Section1' : Section1,
    'Section2' : Section2,
    'Section3' : Section3,
  }

}
</script>