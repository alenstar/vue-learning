<template>
  <div id="app">
    <!--
    <img src="./assets/logo.png">
    <TitleBar></TitleBar>
    <MainContent></MainContent>
    <StatusBar></StatusBar>
    -->
    <vheader class="header"></vheader>
    <div class="main">
      <router-view class="main-wrapper" transition="fade" transition-mode="out-in"></router-view>
    </div>
    <vfooter class="footer"></vfooter>
  </div>
</template>
<script>
// import TitleBar from './components/TitleBar'
// import MainContent from './components/MainContent'
// import StatusBar from './components/StatusBar'

import Vheader from './components/Vheader'
import Vfooter from './components/Vfooter'
import Store from './vuex/store'
export default {
  name: 'app',
  components: {
    // TitleBar,
    // MainContent,
    // StatusBar

    Vheader,
    Vfooter
  },
  store: Store
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

#app {
  display: flex;
  flex-flow: column;
  height: 100%;
}

body a {
  text-decoration: none;
}

.nav a:link,
a:visited {
  color: inherit;
}

body ul,
li,
p {
  list-style: none;
  margin: 0;
  padding: 0;
}

* {
  box-sizing: border-box;
}

.fade-transition {
  transition: all .4s ease;
}

.fade-enter,
.fade-leave {
  opacity: 0;
}

.header,
.footer {
  flex: 0 0 auto;
}

.main {
  flex: 1 0 auto;
  order: 1;
  display: flex;
  justify-content: center;
}

.main-wrapper {
  width: 80%;
  max-width: 80rem;
  transition: all .4s;
}

.footer {
  order: 3;
  display: flex;
  height: 10rem;
}

@media screen and (max-width: 768px) {
  .main-wrapper {
    width: 100%;
  }
  .footer {
    height: 6rem;
  }
}
</style>
