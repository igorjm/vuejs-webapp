<template>
  <footer class="footer">
    <div class="span2">
        <nav class="footer-nav">
            <div class="column">
                <ul>
                    <li><a href="#">Sobre nós</a></li>
                    <li><a href="#">Produtos</a></li>
                    <li><a href="#">Saúde</a></li>
                    <li><a href="#">Dúvidas Frequentes</a></li>
                    <li><a href="#">Onde Encontrar</a></li>
                </ul>
            </div>
            <div class="column">
                <ul>
                    <li><a href="#">Responsabilidade Social</a></li>
                    <li><a href="#">Patrocínio</a></li>
                    <li><a href="#">Imprensa</a></li>
                    <li><a href="#">Trabalhe Conosco</a></li>
                    <li><a href="#">Links Úteis</a></li>
                </ul>
            </div>
            <div class="column">
                <ul>
                    <li><a href="#">Programa Farmácia Popular</a></li>
                    <li><a href="#">Anvisa</a></li>
                    <li><a href="#">Fale Conosco</a></li>
                    <li><a href="#">0800 729 8000 <img src="../../assets/phone-icon.jpg"/></a></li>
                </ul>
            </div>
            <div class="copyright">
                <p>© Copyright 2016 Medley Farmacêutica Ltda. Todos os Direitos Reservados
                </p>
            </div>
        </nav>
    </div>
    <div class="social-media span2">
      <div id="fb-root"></div>
      <div class="fb-page" data-href="https://www.facebook.com/medleybr/" 
       data-small-header="true" data-adapt-container-width="true" data-hide-cover="false"
       data-width="400" data-height="350"
       data-show-facepile="true"><blockquote cite="https://www.facebook.com/medleybr/" 
       class="fb-xfbml-parse-ignore"><a href="https://www.facebook.com/medleybr/">Medley Farmacêutica</a></blockquote></div>
      <br>
      <img src="../../assets/sanofi-icon.jpg" height="50px" alt="Sanofi">
    </div>
  </footer>
</template>

<script>

export default {
  data () {
    return {
      
    }
  },

  created() {
    (function(d, s, id) {
      var js, fjs = d.getElementsByTagName(s)[0];
      if (d.getElementById(id)) return;
      js = d.createElement(s); js.id = id;
      js.src = 'https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v2.12&appId=218363825316154&autoLogAppEvents=1';
      fjs.parentNode.insertBefore(js, fjs);
    }(document, 'script', 'facebook-jssdk'));
  }
}
</script>

<style>
.footer {
    background: #1db2ac url(../../assets/bg-texture.jpg) repeat;
    font-family: "Myriad Pro", "Gill Sans", "Gill Sans MT", Calibri, sans-serif;
    width: 1920px;
    height: 540px;
    padding: 36px 0;
}

.footer-nav {
    float: left;
    margin: 140px auto 250px 268px;
}
.footer-nav .column {
    float: left;
    width: 300px;
}
.footer-nav ul {
  list-style-type: none;
  font-size: 20px;
}
.footer-nav ul li {
  margin-bottom: 12px;
}
.footer-nav a {
  color: #fff;
  font-size: 20px;
  float: bottom;
  text-decoration: none;
}

.copyright {
    text-align: center;
    line-height: 20px;
    font-size: 20px;
    color: #fff;
    margin: 300px auto 250px 268px;
}
.copyright a {
    color: #fff;
    margin-left: 8px;
}

.social-media {
  float: right;
  margin: 150px 80px 0px 0px;
}

.social-media span {
  font-size: 20px !important;
}

.social-media img {
  margin: 100px 100px;
}
</style>