<template>
  <header class="header">
    <div>
      <p class="header__text">NFG</p>
    </div>
    <nav class="header__nav">
      <router-link class="header__section" to="/">Sobre mí</router-link>
      <router-link class="header__section" to="/career">Experiencia</router-link>
      <router-link class="header__section" to="/education">Estudios</router-link>
      <router-link class="header__section" to="/knowledge">Conocimientos</router-link>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    nav: [String],
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5rem;
    position: sticky;
    top: 0;
    left: 0;
    height: auto;
    background-color: inherit;
    &__text {
      margin: 0;
      padding: 0.5rem 1rem;
      font-weight: bold;
      color: $bg-secondary-dark;
    }
    &__section {
      color: $bg-secondary-dark;
      text-decoration: none;
      padding: 0.5rem 1rem;

      &.router-link-exact-active {
        text-decoration: underline;
        font-weight: bold;
      }
    }
  }
</style>
