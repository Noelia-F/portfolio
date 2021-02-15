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
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway&display=swap');
body {
  margin: 0;
}
#app {
  font-family: $font-primary;
  position: relative;
  background-color: $bg-primary;
  display: flex;
  flex-direction: column;
  height: 100vh;
}
.title {
  margin: 0;
  font-size: 2em;
  color: $bg-secondary-dark;
  font-family: $font-secondary;
}
.subtitle {
  margin: 0;
  font-size: 1.5em;
  color: $bg-secondary-dark;
}
.text {
  margin: 0;
  font-size: 1em;
  color: #333;
}
</style>
