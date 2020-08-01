<template>
  <div id="app">
    <Header/>
    <Intro />
    <Terms />
    <Promo />
    <Plans />
    <Global />
    <Feedback />
  </div>
</template>

<script>

import Feedback from './components/Feedback'
import Global from './components/Global'
import Header from './components/Header'
import Intro from './components/Intro'
import Plans from './components/Plans'
import Terms from './components/Terms'

export default {
  name: 'App',
  components: {
    Feedback,
    Global,
    Header,
    Intro,
    Plans,
    Terms
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
