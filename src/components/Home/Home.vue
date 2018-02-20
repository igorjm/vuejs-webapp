<template>
  <div class="home">  
      <h1>QUANDO O ASSUNTO É SAÚDE, CADA DETALHE É IMPORTANTE</h1>
      <p>PRECISÃO, CONTROLE, TRANSPARÊNCIA E A INCASÁVEL DEDICAÇÃO DE CADA DETALHE.
        É ISSO QUE VOCÊ ENCONTRA EM CADA CAIXINHA DA MEDLEY.</p>
    <button class="btn">PLAY <br>VIDEO</button>
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

  .home {
    height: 1080px;
    background: #333 url(../../assets/bg-first.jpg) no-repeat 50% 50%;
    background-size: cover;
    color: #fff;
    text-align: center;
    padding-top: 31px;
    font-family: "Myriad Pro", "Gill Sans", "Gill Sans MT", Calibri, sans-serif;
  }

  .home h1 {
    font-size: 60px;
    font-weight: 400;
    max-width: 1000px;
    margin: 350px auto 30px;
  }

  .home p {
    font-size: 15px;
    max-width: 620px;
    margin: 0 auto 51px;
  }

  .btn {
    font-size: 13px !important;
    margin: 150px;
    width: 130px !important;
    height: 130px!important;
    position: relative;
    border: none;
    border-radius: 50%;
    color: #fff;
    background: linear-gradient(to right, #1bb0aa , #71bd66);
    cursor:pointer;
  }

</style>