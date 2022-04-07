<template>
  <div id="app">
    <h1> {{ 1 + 2 + 3 + 4 }} </h1>
    <h1>with Methods {{ counter() }} </h1>
    <h1>with Methods {{ counterParams(1, 3, 5) }} </h1>
    <h1>multiple methods {{ multiply(baseValue) }} </h1>
  </div>
</template>

<script>

export default {
  name:'app',
  data(){
    return{
      baseMultiple: 5,
      baseValue: 10
    }
  },
  methods:{
    counter(){
      return 2 + 2 + 2 + 2
    },
    counterParams(a, b, c){
      return a * b * c
    },
    multiply (num) {
      return this.baseMultiple * num
    }
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
