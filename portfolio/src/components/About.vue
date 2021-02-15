<template>
  <div class="about">
    <section class="about__introduction">
      <h1 class="title">Noelia Frontón García</h1>
      <h2 class="subtitle">Front-End Developer</h2>
      <p class="text">Texto descriptivo aquí...</p>
    </section>
    <section class="about__info">
      <div class="about_card"></div>
      <div class="about_card"></div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'About',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.about {
  padding: 2rem;
  flex: 2;
  &__introduction {
    margin-bottom: 2rem;
  }
  &__info {
    display: grid;
    grid-template-columns: repeat( auto-fit, minmax(250px, 1fr) );
    gap: 2rem;
  }
  &_card {
    background-color: #c7c7c7;
    box-shadow: 1px 1px 3px rgba(51,51,51,0.99);
    padding: 2rem;
  }
}
</style>
