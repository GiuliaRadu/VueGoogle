<template>
  <div id="app">
    <GooglePage/>
  </div>
</template>

<script>
import GooglePage from './components/GooglePage.vue'

export default {
  name: 'App',
  components: {
    GooglePage
  }
}
</script>

<style>

*{
  margin:0;
  padding:0;
}
html {
  width:100vw;
  height:100vh;
}

body{
  width:100%;
  height:100%;
  min-height: 100vh;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width:100%;
  height:100%;
}
</style>
