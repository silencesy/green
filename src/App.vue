<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from './components/Home'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
#app {
  font-family: Arial;
  max-width: 750px;
  margin: 0 auto;
}
* {
  margin: 0;
  padding: 0;
}
</style>
