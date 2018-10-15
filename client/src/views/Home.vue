<template>
  <div id="home">
    <section id="hero">
      <Nav />
        <div class="container">
          <div class="row cards">
            <div class="column column-offset-50">
              <h2>You can find me here</h2>
              <HeroCard title="View My Projects" icon="project-bar.svg" />
              <HeroCard title="Listen To My Podcast" icon="podcast-bar.svg" />
              <HeroCard title="Read My Blog" icon="blog-bar.svg" />
              <HeroCard title="Follow Me" icon="social-bar.svg" />
            </div>
          </div>
        </div>
    </section>
    <section id="about">
      <PageHeader subtitle="I am a Canadian" title="Professor & Developer" text="My general attitude to life is to enjoy every minute of every day. I never do anything with a feeling of, 'Oh God, I've got to do this today.' - Richard Branson" />
    </section>
    <section id="activity">
      <PageSubHeader subtitle="What have I been up to?" title="Recenty Activity" />
      <div class="container activity-cards">
        <ActivityCard image="../assets/images/social-bar.svg" 
                      title="This is a tweet title" 
                      text="Consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam…"
                      source="Twitter"
                      date="October 15 2018"
                      link="https://twitter.com"
        />
        <p id="last-updated-text"><span>Last updated:</span> 3 hours ago</p>
      </div>
    </section>
    <section id="footer-block">
      <Footer />
    </section>
  </div>
</template>

<script>
  import Nav from '@/components/Nav.vue'
  import HeroCard from '@/components/HeroCard.vue'
  import PageHeader from '@/components/PageHeader.vue'
  import PageSubHeader from '@/components/PageSubHeader.vue'
  import ActivityCard from '@/components/ActivityCard.vue'
  import Footer from '@/components/Footer.vue'

  export default {
    name: 'home',
    components: {
      Nav,
      HeroCard,
      PageHeader,
      PageSubHeader,
      ActivityCard,
      Footer
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

  .row.cards {
    margin-top: 18px;
  }
  .row.cards h2 {
    margin-top: 59px;
    margin-bottom:18px;
    text-align: center;
    color: var(--white-color);
  }
  @media(max-width: 768px) {
    .row .column.column-offset-50 {
      margin: 0;
    }
    .row.cards h2 {
      margin-top: 0;
    }
  }

  #about {
    margin-top: -100px;
    margin-bottom: 89px;
  }
  @media(max-width: 768px) {
    #about {
      margin-top: 0px;
    }
  }

  #activity .activity-cards {
    margin-top: 43px;
  }

  #last-updated-text {
    color: var(--light-color);
    font-size: 20px;
    line-height: 25px;
    text-align: center;
    margin-top: 34px;
  }

  #last-updated-text span {
    font-weight: bold;
  }
</style>
