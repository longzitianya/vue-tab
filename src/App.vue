<template>
  <div id="app">
    <tab :tabtitles="tabtitles" 
    :current-page="3">
    <div class="tab-content-container">
      <button onclick="alert(2)">click</button>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <div>hahaha1</div>
      <img src="./assets/logo.png">
      <div>hahaha1</div>
      <div>hahaha1</div>
    </div>
    <div class="tab-content-container">
      bajian2
    </div>
    <div class="tab-content-container">
      bajian3
    </div>
    <div class="tab-content-container">
      bajian4
    </div>
  </tab>

  <br>
  <br>
  <br>
  <br>
  <div>allow different height、verticle scroll、<b>disable slide below:</b></div>
  
  <br>

  <tab :tabtitles="tabtitles2"
  :slidable="false">
  <div style="height: 200px;background-color: green" class="tab-content-container">
    hahaha1
    <img src="./assets/logo.png">
    <div>hahaha1</div>
    <div>hahaha1</div>
  </div>
  <div style="background-color: #999" class="tab-content-container">
    bajian2
  </div>
  <div class="tab-content-container">
    bajian3
  </div>
</tab>

  <br>
  <br>
</div>
</template>

<script>
  import tab from './components/vue-tab'

  export default {
    components: {
      tab
    },
    data(){
      return {
        'tabtitles':['bajian','github','bajian','github'],
        'tabtitles2':['bajian','github','bajian'],
      }
    }
  }
</script>

<style>
  html {
    height: 100%;
  }

  *{
    margin: 0px;
    padding: 0px;
  }

/*  body {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
  }*/

  .tab-content-container{
    width: 99%;
    height: 200px;
    margin: 0px auto;
  }

  #app {
    color: #2c3e50;
    margin-top: 50px;
    max-width: 500px;
    width: 100%;
    font-family: Source Sans Pro, Helvetica, sans-serif;
    /*text-align: center;*/
    margin: 0 auto
  }

  img{
    width: 98%
  }


/*TO change the active color u like
    .tab-title.active,.tab-title:active {
        border-bottom: 2px solid #36acf4;
        color: #36acf4;
      }*/
    </style>
