<template>
  <footer class="footer">
    <p class="footer__text">Footer</p>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    nav: [String],
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .footer {
    padding: 2rem;
    height: auto;
    min-height: 100px;
    background-color: #424B54;
    &__text {
      color: #fff;
    }
  }
</style>
