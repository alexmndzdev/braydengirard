<template>
  <div id="footer">
    <div id="main-footer">
      <h1>Brayden Girard</h1>
      <div id="social-icons">
      <a href="">
        <img src="../assets/images/twitter-footer.svg" alt="Twitter" />
      </a>
      <a href="">
        <img src="../assets/images/github-footer.svg" alt="GitHub" />
      </a>
      </div>
    </div>
    <div id="sub-footer">
      <p>© Brayden Girard 2018. All Rights Reserved.</p>
    </div>
  </div>
</template>
<style scoped>
  #footer {
    height: 398px;
    background-image: url("../assets/images/footer-bg.jpg");
    background-size: cover;
    background-position: center; 
  }
  #main-footer {
    height: 348px;
    padding: 165px 0 80px;
  }
  #sub-footer {
    height: 50px;
    background-color: rgba(38,38,38,0.2);
  }
  #sub-footer p {
    text-align: center;
    line-height: 50px;
    font-size: 16px;
    color: var(--white-color);
  }
  #footer h1 {
    color: #FFFFFF;
    font-size: 47px;
    font-weight: bold;
    line-height: 59px;
    text-align: center;
  }
  #social-icons {
    display: block;
    width: 167px;
    margin: 13px auto 0;
  }
  #footer img {
    height: 30px;
    display: inline-block;
    margin: 0 25px;
  }
</style>