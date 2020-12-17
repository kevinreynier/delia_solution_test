<template>
  <div class="scoreBoard">
      Score : {{score}}
  </div>
</template>

<script>

export default {
  name: 'ScoreBoard',
  props: {
    score: Number
  },
  data() {
      return {    
      }
  },
  computed: {
  },
  methods: {
  }

}
</script>


<style scoped>
</style>