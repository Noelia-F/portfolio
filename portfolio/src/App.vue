<template>
  <div id="app">
    <Header/>
    <router-view/>
    <Footer/>
  </div>
</template>
<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
  }
}
</script>
<style lang="scss">
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  position: relative;
  background-color: #EBCFB2;
  display: flex;
  flex-direction: column;
  height: 100vh;
}
.title {
  margin: 0;
  font-size: 2em;
}
.subtitle {
  margin: 0;
  font-size: 1.5em;
}
.text {
  margin: 0;
  font-size: 1em;
}
</style>
