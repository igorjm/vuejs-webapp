<template>
  <div class="about">
    <h1>POR QUE ESCOLHER A MEDLEY?</h1>
    <p>Alto padrão de qualidade e preço acessível.</p>
    <div class="slideshow-container">
        <div class="slide fade">
            <div class="span2">
                <h3>PRECISÃO</h3>
                <p>A saúde está na precisão e no controle em cada etapa
                dos nossos processos. Está na exigência que nos faz
                ir muito além do esperado. </p>
            </div>
            <div class="span2">
                <div class="circle-precisao">    
                </div>
            </div>
        </div>
        <!-- <div class="slide fade">
            <div class="span2">
                <h3>CONTROLE</h3>
                <p>Fazemos testes além do exigido para que você leve
                o melhor medicamento para casa. </p>
            </div
            <div class="span2">
                <div class="circle-controle">    
                </div>
            </div
        </div>
        <div class="slide fade">
            <div class="span2">
                <h3>DEDICAÇÃO</h3>
                <p>Pensar em cada detalhe, por menor que seja.
                Isso não faz diferença apenas na sua vida:
                faz uma diferença para produzir cada medicamento. </p>
            </div>
            <div class="span2">
                <div class="circle-dedicacao">    
                </div>
            </div>
        </div>
        <div class="slide fade">
            <div class="span2">
                <h3>CUIDADO</h3>
                <p>A saúde está na precisão e no controle em cada etapa
                dos nossos processos. Está na exigência que nos faz
                ir muito além do esperado. </p> 
            </div>
            <div class="span2">
                <div class="circle-cuidado">    
                </div>
            </div>
        </div> -->
    </div>
    <div class="dots">
        <span class="dot" onclick="currentSlide(1)"></span>
        <span class="dot" onclick="currentSlide(2)"></span>
        <span class="dot" onclick="currentSlide(3)"></span>
        <span class="dot" onclick="currentSlide(4)"></span>
    </div>
  </div>
</template>

<script>

export default {
    data () {
        var slideIndex = 1;
    },

    created() {
        showSlides(slideIndex);
    },

    methods: {
        plusSlides(n) {
            showSlides(slideIndex += n);
        },

        currentSlide(n) {
            showSlides(slideIndex = n);
        },

        showSlides(n) {
            var i;
            var slides = document.getElementsByClassName("slide");
            var dots = document.getElementsByClassName("dot");
            if (n > slides.length) {slideIndex = 1}    
            if (n < 1) {slideIndex = slides.length}
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";  
            }
            for (i = 0; i < dots.length; i++) {
                dots[i].className = dots[i].className.replace(" active", "");
            }
            slides[slideIndex-1].style.display = "block";  
            dots[slideIndex-1].className += " active";
        }
    }

}

</script>

<style>
.about {
    height: 985px;
    background: #fff no-repeat 50% 50%;
    background-size: cover;
    color: #333;
    text-align: center;
    padding-top: 31px;
}

.about h1 {
    text-align: left;
    color: #1db2ab;
    font-size: 60px;
    font-weight: 400;
    margin: 250px 0px 0px 250px;
    max-width: 300px;
}

.about h3 {
    text-align: left;
    color: #1db2ab;
    font-size: 35px;
    font-weight: 400;
    margin: 100px 0px 0px 250px;
    max-width: 300px;
}

.about p {
    color: black;
    font-size: 20px;
    max-width: 500px;
    margin: 15px 0px 0px 220px;
}

.slideshow-container {
    margin: 100px 0px 0px 250px;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #fff;
  border:1px solid #2cb7b1;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #19b1aa;
}

.dots {
    text-align: left;
    margin: 150px 0px 0px 300px;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}

.slide p {
    text-align: left;
    margin:20px 0px 0px 50px;
    width:600px;
}

.slide h3 {
    margin:50px 0px 30px 50px;
}

.about .circle-precisao {
    width:700px;
    height:700px;
    border:1px solid #2cb7b1;
    border-radius:100%;
    position: absolute;
    z-index: 153;
    margin:-600px 0px 0px 800px;
    background-color: #fff;
    background-image: url('../../assets/precisao.jpg');
    background-size: 250px;
    background-repeat: no-repeat;
    background-position: 50%;
}

.about .circle-controle {
    width:700px;
    height:700px;
    border:1px solid #2cb7b1;
    border-radius:100%;
    position: absolute;
    z-index: 153;
    margin:-600px 0px 0px 800px;
    background-color: #fff;
    background-image: url('../../assets/precisao.jpg');
    background-size: 250px;
    background-repeat: no-repeat;
    background-position: 50%;
}

.about .circle-dedicacao {
    width:700px;
    height:700px;
    border:1px solid #2cb7b1;
    border-radius:100%;
    position: absolute;
    z-index: 153;
    margin:-600px 0px 0px 800px;
    background-color: #fff;
    background-image: url('../../assets/precisao.jpg');
    background-size: 250px;
    background-repeat: no-repeat;
    background-position: 50%;
}

.about .circle-cuidado {
    width:700px;
    height:700px;
    border:1px solid #2cb7b1;
    border-radius:100%;
    position: absolute;
    z-index: 153;
    margin:-600px 0px 0px 800px;
    background-color: #fff;
    background-image: url('../../assets/precisao.jpg');
    background-size: 250px;
    background-repeat: no-repeat;
    background-position: 50%;
}

</style>