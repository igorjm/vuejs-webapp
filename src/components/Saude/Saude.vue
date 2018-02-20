<template>
  <div class="saude">
      <div class="saude-1 span2">
      </div>
      <div class="saude-2 span2">
      </div>
      <div class="saude-3 span2">
      </div>
      <div class="saude-4 span2">
      </div>
  </div>
</template>

<script>

export default {

  data () {
    return {
      
    }
  }
}
</script>

<style>

  .saude {
    height: 1080px;
    background-size: cover;
    color: #fff;
    text-align: center;
    padding-top: 31px;
    font-family: "Myriad Pro", "Gill Sans", "Gill Sans MT", Calibri, sans-serif;
  }

  .saude-1 {
      background: #333 url(../../assets/saude-1.jpg) no-repeat 50% 50%;
  }

  .saude-2 {
      background: #333 url(../../assets/saude-2.jpg) no-repeat 50% 50%;
  }

  .saude-3 {
      background: #333 url(../../assets/saude-3.jpg) no-repeat 50% 50%;
  }

  .saude-4 {
      background: #333 url(../../assets/saude-4.jpg) no-repeat 50% 50%;
  }

</style>