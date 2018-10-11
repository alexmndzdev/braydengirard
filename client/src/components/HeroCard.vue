<template>
  <div id="card">
    <img :src="icon" :alt="title" />
    <h2>{{ title }}</h2>
  </div>
</template>
<script>
  export default {
    props: ['icon', 'title']
  }
</script>
<style scoped>
  #card {
    height: 88px;
    border-radius: 4px;
    background-color: #FFFFFF;
    box-shadow: 0 0 10px 0 rgba(0,0,0,0.2);
    margin: 10px 0;
    text-align: center;
  }
  #card h2 {
      color: #9B9B9B;	
      font-size: 24px;	
      line-height: 88px;	
  }
  #card img {
    float: left;
  }

  @media (max-width: 768px) {
    #card {
      height: 75px;
    }
    #card h2 {
      font-size: 20px;	
      line-height: 75px;
      margin-top: 23px;
    }
  }
</style>