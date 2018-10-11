<template>
  <div id="page-sub-header" class="container">
    <h2>{{ subtitle }}</h2>
    <h1>{{ title }}</h1>
  </div>
</template>
<script>
  export default {
    props: ['subtitle', 'title']
  }
</script>
<style scoped>

</style>