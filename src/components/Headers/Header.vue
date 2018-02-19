<template>
  <div class="main-header">
    <div class="logo-header"><img src="../../assets/medley_logo.png" height="30" width="85" alt=""/></div>
    <div class="sidebar-menu">
      <button class="menu-button" id="menu-button">&#9776;</button>
    </div>
    <div class="header-search">
      <img src="../../assets/search_icon.png" />
      <input type="text" placeholder="O que você está procurando?">
    </div>
  </div>
</template>

<script>

function openMenu(){
  console.log("abriu");
}

export default {
  data () {
    return {

    }
  }
}
</script>

<style>
  .main-header {
    background: #1db2ac url(../../assets/bg-texture.jpg) repeat;
    width: 1920px;
    height: 100px;
  }

  .logo-header {
    float: left;
    margin: 34px 0px 43px 93px;
  }

  .sidebar-menu {
    float: right;
    display: inline;
    margin: 30px 90px 40px 0px;
    outline:none;
    z-index:10000000000000;
  }

  .sidebar-menu button {
    background:none;
    position:relative;
    color:#fcfcfc;
    border:0;
    font-size:2em;
    font-weight:bold;
    cursor:pointer;
  }

  .header-search {
    position: relative;
    color: #aaa;
    font-size: 20px;
    float: right;
    display: inline;
    margin: 38px 200px 29px 0px;
    outline:none;
    z-index:10000000000000;
  }

  .header-search input {
    width: 431px;
    height: 32px;
    font-size: 16px;

    background: #fcfcfc;
    border: 1px solid #aaa;
    border-radius: 15px;
    box-shadow: 0 0 3px #ccc, 0 10px 15px #ebebeb inset;
  }

  .header-search input { text-indent: 32px;}
  .header-search img { 
    position: absolute;
    top: 8.5px;
    right: 15px;
  }
</style>