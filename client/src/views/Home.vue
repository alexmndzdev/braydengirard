<template>
  <div id="home">
    <section id="hero">
      <Nav />
        <div class="container">
          <div class="row cards">
            <div class="column column-offset-50">
              <p>You can find me here</p>
              <HeroCard title="View All Projects" icon="../assets/images/project-bar.svg" />
              <HeroCard title="View All Projects" icon="../assets/images/podcast-bar.svg" />
              <HeroCard title="View All Projects" icon="../assets/images/blog-bar.svg" />
              <HeroCard title="View All Projects" icon="../assets/images/social-bar.svg" />
            </div>
          </div>
        </div>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import Nav from '@/components/Nav.vue'
import HeroCard from '@/components/HeroCard.vue'

export default {
  name: 'home',
  components: {
    Nav,
    HeroCard
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

  .row.cards {
    margin-top: 18px;
  }

  .row.cards p {
    margin-top: 59px;
    line-height: 38px;
    text-align: center;
    color: var(--white-color);
    font-size: 30px;
  }

  @media (max-width: 768px) {
    #hero { 
      background-image: url("../assets/images/hero-small.jpg");
    }
    .row .column.column-offset-50 {
      margin: 0;
    }
    .row.cards p {
      margin-top: 20px;
    }
  }
</style>
