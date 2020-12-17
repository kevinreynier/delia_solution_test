<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <body>
      <Shape v-for="n in 5" :key="n" @circleIsClicked="addScore"/>
    </body>
    <footer>
      <ScoreBoard :score="score" />
    </footer>
  </div>
</template>

<script>
import Shape from '@/components/Shape.vue'
import ScoreBoard from '@/components/ScoreBoard.vue'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    Shape,
    ScoreBoard
  },
  data() {
    return {
      score :0
    }
  },
  methods: {
    addScore(){
      this.score ++
    }
  }
}
</script>


<style scoped>
h3 {
  margin: 40px 0 0;
}
body {
  background-color: beige;
  height: 500px;
  width: 1000px;
}
</style>
