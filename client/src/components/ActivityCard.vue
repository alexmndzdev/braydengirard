<template>
  <div id="activity-card">
    <div class="row">
      <div id="icon-view" class="column column-20">
        <img id="icon" :src="image" :alt="source" />
      </div>
      <div id="text-view" class="column column-60">
        <h1>{{ title }}</h1>
        <p>{{ text }}</p>
        <p id="source-desktop">Source: <span>{{ source }}</span></p>
        <p id="source-mobile"><a :href="link" >View</a></p>
      </div>
      <div id="date-view" class="column column-20">
        <p>Posted {{ date }}</p>
        <div id="view-button"><a :href="link">View</a></div>
      </div>
    </div>
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
    padding: 11px 33px;
  }
  h1 {
    font-size: 42px;
    line-height: 52px;
  }

  #icon-view {
    padding-right: 33px;
  }

  #text-view {
    border-left: 1px solid rgba(0,0,0,0.2);
    padding-left: 33px;
    padding-right: 33px;
  }

  #source-desktop, #source-mobile {
    font-size: 13px;
    font-style: italic;
    font-weight: 300;
    line-height: 24px;
    margin-top: 9px;
  }
  #source-mobile a {
    color: #00C887;
  }
  #source-mobile {
    display: none;
  }
  #source-desktop span {
    color: #00C887;
  }

  #icon {
    display: block;
    margin: 0 auto;
  }

  #date-view {
    text-align: right;
    margin-top: 17px;
  }

  #view-button {
    margin-top: 33px;
  }
  #view-button a {
    color: #00C887;
    font-size: 24px;
    line-height: 31px;
  }

  @media (max-width: 768px) {
    h1 {
      font-size: 24px;
      line-height: 30px;
    }
    #source-mobile { 
      display: block;
    }
    #source-desktop {
      display: none;
    }
    #icon {
      float: left;
    }
    #date-view {
      display: none;
    }
    #activity-card {
      padding: 8px 15px;
    }
    #text-view {
      border-left: 1px solid rgba(0,0,0,0.2);
      padding-left: 10px;
      padding-right: 10px;
    }
  }
</style>