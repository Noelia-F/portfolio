<template>
  <div class="home">
    <About msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import About from '@/components/About.vue'

export default {
  name: 'Home',
  components: {
    About
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .home {
    flex: 1;
  }
</style>
