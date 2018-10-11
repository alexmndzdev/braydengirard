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
    --dark-color: #272727;
    --light-color: #9B9B9B;
  }
  h1 {
    color: #272727;
    font-size: 62px;
    font-weight: bold;
    line-height: 78px;
    margin-bottom: 0;
  }
  h2 {
    color: #9B9B9B;
    font-size: 30px;
    line-height: 38px;
    margin-bottom: 0;
  }
  p {
	  color: #9B9B9B;
	  font-size: 18px;
	  line-height: 21px;
    margin-bottom: 0;
  }

  @media (max-width: 768px) {
    h1 {
      color: #272727;
      font-size: 40px;
      font-weight: bold;
      line-height: 54px;
      margin-bottom: 0;
    }
    h2 {
      color: #9B9B9B;
      font-size: 22px;
      line-height: 35px;
      margin-bottom: 0;
    }
    p {
      font-size: 15px;
      line-height: 16px;
    }
  }
</style>
