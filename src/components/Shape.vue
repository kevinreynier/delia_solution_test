<template>
  <div class="circle" 
        style="top: 200px; left: 100px; "
        v-show="!isClicked" 
        @click="circleClicked"> </div>
</template>


<script>
export default {
  name: 'Circle',
  data() {
      return {   
          isClicked : false
      }
  },
  computed: {
  },
  methods: {
      circleClicked() {
          console.log("zrf")
          this.isClicked = !this.isClicked
          this.$emit("circleIsClicked")
      }
  }
}
</script>

<style scoped>
.circle{
    position: absolute;
    background-color:brown;   
    padding: 60px;
    margin: 20px;
    border-radius: 50%;
    float: left;
    shape-outside: margin-box;
}
</style>