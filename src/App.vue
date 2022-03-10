<template>
  <div>
    <button type="button" @click="showAlert">Click Me</button>
  </div>
</template>

<script>
import {greet} from 'rustfiles'

export default {
  name: 'App',
  components: {
  },
  methods:{
    showAlert(){
      greet("Hello world from vue via rust webassembly")
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
