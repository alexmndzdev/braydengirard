<template>
  <div id="activity-card">
    
  </div>
</template>
<script>
  export default {
    props: ['image', 'title', 'text', 'source', 'date', 'link']
  }
</script>
<style scoped>
  #activity-card {
    height: 152px;
    border-radius: 4px;
    background-color: var(--white-color);
    box-shadow: 0 0 10px 0 rgba(0,0,0,0.2);
  }
</style>