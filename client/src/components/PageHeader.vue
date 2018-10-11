<template>
  <div id="page-header" class="container">
    <div class="row">
      <div class="column column-60 column-offset-20">
        <h2>{{ subtitle }}</h2>
        <h1>{{ title }}</h1>
        <p>{{ text }}</p>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    props: ['subtitle', 'title', 'text']
  }
</script>
<style scoped>
  #page-header {
    text-align: center;
  }
  #page-header p {
    line-height: 24px;
    margin-top: 18px;
  }
  @media(max-width: 768px) {
    .row .column.column-60 {
      flex: 0 0 100%;
      max-width: 100%;
    }
    .row .column.column-offset-20 {
      margin: 0;
    }
    #page-header p {
      line-height: 19px;
    }
  }
</style>