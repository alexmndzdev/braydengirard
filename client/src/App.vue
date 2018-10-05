<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css?family=Roboto:300,300italic,700,700italic');
  @import url('https://cdn.rawgit.com/necolas/normalize.css/master/normalize.css');
  @import url('https://cdn.rawgit.com/milligram/milligram/master/dist/milligram.min.css');
  @import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro:400,700');

  #app {
    font-family: 'Source Sans Pro', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    --white-color: white;
    --black-color: black;
  }
</style>
