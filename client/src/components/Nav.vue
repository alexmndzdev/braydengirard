<template>
  <div id="nav" :class="{ 'nav-background': solid }">
    <div class="container">
      <div class="row desktop-only">
        <div class="column column-40 logo-text"><router-link to="/">Brayden Girard</router-link></div>
        <div class="column column-30">
          <router-link to="/projects">Projects</router-link>
          <router-link to="/podcasts">Podcasts</router-link>
          <router-link to="/blog">Blog</router-link>
        </div>
        <div class="column column-20 contact"><router-link to="/contact">Contact</router-link></div>
      </div>
      <div class="row mobile-only">
        <div class="column logo-text logo-text-mobile"><router-link to="/">Brayden Girard</router-link></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  props: {
    solid: Boolean
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #nav {
    padding: 10px;
    text-align: left;
  }

  .nav-background {
    background-color: var(--black-color);
  }

  #nav a {
    font-size: 18px;
    color: var(--white-color);
    margin: 0 25px;
    line-height: 50px;
    vertical-align: middle;
  }

  #nav .logo-text a {
    font-size: 40px;
    line-height: 50px;
    font-weight: bold;
  }

  #nav .contact {
    text-align: right;
  }

  .desktop-only {
    display: flex;
  }
  
  .mobile-only {
    display: none;
  }

  @media (max-width: 768px) {
    .desktop-only {
      display: none;
    }
    
    .mobile-only {
      display: flex;
    }

    #nav .logo-text-mobile a {
      font-size: 38px;
      margin: 0;
    }

    #nav .logo-text-mobile {
      text-align: center;
    }
  }
</style>
