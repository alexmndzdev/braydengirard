<template>
  <div id="home">
    <section id="hero">
      <Nav />
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import Nav from '@/components/Nav.vue'

export default {
  name: 'home',
  components: {
    Nav
  }
}
</script>

<style scoped>
  #hero {
    height: 805px;
    background-image: url("../assets/images/hero.jpg");
    background-size: cover;
    background-position: center; 
  }

  @media (max-width: 768px) {
    #hero { 
      background-image: url("../assets/images/hero-small.jpg");
    }
  }
</style>
