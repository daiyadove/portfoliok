<template>
  <div id="app">
    <h1>間に合いませんでした!Twitterに飛びます!</h1>
    <a href="https://twitter.com/flowphantom">Twitter</a>
  </div>
</template>

<script>
  window.location.href = 'https://twitter.com/flowphantom';
export default {
    name: 'app',
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
