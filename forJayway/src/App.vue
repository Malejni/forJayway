<template>
  <div id="app">
    <router-view/>
    <footer></footer>
  </div>
</template>

<script>
import Footer from './components/footer'

export default {
  name: 'App',
  component: Footer
}
</script>

<style>
html {
   height: 100%;
   box-sizing: border-box;
}
body {
  margin: 0;
  min-height: 100%;
  display: grid;
  box-sizing: border-box;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
