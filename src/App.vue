<template>
  <div id="app">
    <img src="./assets/logo.png">
    <TitleBar></TitleBar>
    <MainContent></MainContent>
    <StatusBar></StatusBar>
  </div>
</template>
<script>
import TitleBar from './components/TitleBar'
import MainContent from './components/MainContent'
import StatusBar from './components/StatusBar'

export default {
  name: 'app',
  components: {
    TitleBar,
    MainContent,
    StatusBar
  }
}
</script>
<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 4px;
}
</style>
