<template>
  <div class="main_container">
    <!-- Header Image Container -->
    <div class="jumbotron">
      <div class="container header_container">
        <img src="../assets/images/oekotex_de.png" class="header_img_div">
        <div class="row align-items-center">
          <div class="col-sm-12 col-md-12 col-lg-5 header_text_div">
            <h1>Entdecke unsere Hautfreundlichkeit</h1>
            <p class="text-uppercase">
              <a class="btn border-w-2 btn-md">Jetzt Deine Größe wählen</a>
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- Test Package Container -->
    <div class="container-fluid text-center test_package_container">
      <div class="container-fluid">
        <div class="row test_package_row">
          <div class="col-lg-7 col-md-7 mb-20">
            <div class="test_package_img_div">
              <img :src="imgurl" class="testpaket_img" id="img_id">
              <img src="../assets/images/oekotex_de.png" class="oekotex_img">
            </div>
          </div>
          <div class="col-lg-5 col-md-5 mb-20 text-left">
            <h3>Unser gratis Testpaket</h3>
            <p>WÄHLE DEINE GRÖSSE</p>
            <div class="row" id="selective_btn_id">
              <button class="selective_btn active" @click="changeImage(10)">
                <span class="selective_btn_span">1</span>
                <br>
                <span class="selective_btn_kg_span">(2-3 KG)</span>
              </button>
              <button class="selective_btn" @click="changeImage(20)">
                <span class="selective_btn_span">2</span>
                <br>
                <span class="selective_btn_kg_span">(3-4 KG)</span>
              </button>
              <button class="selective_btn" @click="changeImage(30)">
                <span class="selective_btn_span">3</span>
                <br>
                <span class="selective_btn_kg_span">(4-7 KG)</span>
              </button>
              <button class="selective_btn" @click="changeImage(40)">
                <span class="selective_btn_span">4</span>
                <br>
                <span class="selective_btn_kg_span">(7-10 KG)</span>
              </button>
              <button class="selective_btn" @click="changeImage(50)">
                <span class="selective_btn_span">5</span>
                <br>
                <span class="selective_btn_kg_span">(10-12 KG)</span>
              </button>
            </div>
            <p>Teste jetzt unsere Windeln und Feuchttücher - In Größe 1 - 3 enthält unser Testpaket unsere Feuchttücher mit 99 % Wasser, ab Gr. 4 erhältst Du unsere Sensitiven Feuchttücher. Wir zahlen die Produkte, Du nur den Versand.</p>
            <ul>
              <li
                style="color:#00afab;"
              >Automatischer Übergang ins jederzeit kündbare Windel-Abo für 49,50 € pro Lieferung.</li>
              <li>
                Preise inkl. MwSt., ggf. zzgl.
                <span style="color:#00afab;">Versandkosten</span>
              </li>
            </ul>
            <button class="cart_btn">In den Warenkorb legen</button>
          </div>
        </div>
      </div>
    </div>
    <!-- Subscription Container -->
    <div class="container-fluid text-center subscription_container">
      <div class="container">
        <div class="row subscription_row">
          <h1>Wie es funktioniert</h1>
        </div>
        <div class="row">
          <div class="col-lg-4 col-md-4">
            <div class="subscription-icons-item mx-auto mb-5 mb-lg-0 mb-lg-3">
              <div class="subscription-icons-icon d-flex">
                <img src="../assets/images/lillydoo-your-trialbox-icon.svg">
              </div>
              <h4>DEIN TESTPAKET</h4>
              <p class="subcription_p mb-0">
                Wir schenken Dir die Produkte,
                Du übernimmst nur das Porto.
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-4">
            <div class="subscription-icons-item mx-auto mb-5 mb-lg-0 mb-lg-3">
              <div class="subscription-icons-icon d-flex">
                <img src="../assets/images/lillydoo-your-flexibility-icon.svg">
              </div>
              <h4>DEINE FLEXIBILITÄT</h4>
              <p class="subcription_p mb-0">
                Erste Monatsbox nach 14 Tagen für 49,50 € erhalten.
                Oder noch vor der ersten Lieferung kündigen.
              </p>
            </div>
            <p>
              <a>
                Erfahre hier mehr über das
                <br>
              </a>
              <a>LILLYDOO Windel-Abo.</a>
            </p>
          </div>
          <div class="col-lg-4 col-md-4">
            <div class="subscription-icons-item mx-auto mb-0 mb-lg-3">
              <div class="subscription-icons-icon d-flex">
                <img src="../assets/images/lillydoo-your-subscription-icon.svg">
              </div>
              <h4>DEINE MONATSBOX</h4>
              <p class="subcription_p mb-0">
                Jederzeit Designs oder Lieferintervalle anpassen
                oder die Windelgröße ändern.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Diaper Container -->
    <div class="container-fluid text-center diaper_container">
      <div class="container-fluid">
        <div class="row diaper_row">
          <h1>Dein Testpaket enthält</h1>
        </div>
        <div class="row diaper_row">
          <div class="col-lg-6 col-md-6 mb-20">
            <div class="media">
              <div class="media-left">
                <img
                  src="../assets/images/lillydoo-little-blowballs-design-preview-tp.jpg"
                  class="media-object"
                >
              </div>
              <div class="media-body text-left">
                <h4 class="media-heading">10 LILLYDOO WINDELN</h4>
                <ul class="diaper_ul">
                  <li>0 % Parfüme & Lotionen, 100 % LILLYDOO Schutz</li>
                  <li>Extra weich und mit idealer Passform</li>
                </ul>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-6 mb-20">
            <div class="media">
              <div class="media-left">
                <img :src="waterWipesImgurl" class="media-object" id="waterWipesImg_id">
              </div>
              <div class="media-body text-left">
                <h4 class="media-heading" id="waterWipesText_id">15 FEUCHTTÜCHER MIT 99 % WASSER</h4>
                <ul class="diaper_ul">
                  <li>0 % Parfüme & PEGs, 100 % biologisch abbaubar</li>
                  <li
                    id="waterWipesNaturalText_id"
                  >Natürlich rein, extra mild, Alternative zu "Wasser & Watte"</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      imgurl: require('../assets/images/lillydoo-testpaket-10.jpg'),
      waterWipesImgurl: require('../assets/images/water-wipes-15-small (1).jpg')
    }
  },

  methods: {
    // Change Image and text Function
    changeImage(event) {
      // TestPacket Image Change Variables

      var path = require('../assets/images/lillydoo-testpaket-' +
        event +
        '.jpg')
      document.getElementById('img_id').src = path

      // Diaper Image and Text Change variables

      var waterWipesPath = require('../assets/images/sensitive-wipes-15-small.jpg')
      var waterWipes_text = '15 FEUCHTTÜCHER MIT 99 % WASSER'
      var sensitiveWipes_text = '15 SENSITIVE FEUCHTTÜCHER'
      var waterWipesNatural_text =
        'Natürlich rein, extra mild, Alternative zu "Wasser & Watte"'
      var waterWipesThick_text = 'Extra dickes und kompostierbares Tuch'

      // Diaper Image and Text Change Functions
      if (event === 40 || event === 50) {
        document.getElementById('waterWipesImg_id').src = waterWipesPath
        document.getElementById(
          'waterWipesText_id'
        ).innerHTML = sensitiveWipes_text
        document.getElementById(
          'waterWipesNaturalText_id'
        ).innerHTML = waterWipesThick_text
      } else {
        document.getElementById(
          'waterWipesImg_id'
        ).src = require('../assets/images/water-wipes-15-small (1).jpg')
        document.getElementById('waterWipesText_id').innerHTML = waterWipes_text
        document.getElementById(
          'waterWipesNaturalText_id'
        ).innerHTML = waterWipesNatural_text
      }

      // Active Class for highlighting button color
      var selectiveButton = document.getElementById('selective_btn_id')
      var buttons = selectiveButton.getElementsByClassName('selective_btn')
      for (var i = 0; i < buttons.length; i++) {
        buttons[i].addEventListener('click', function() {
          var current = document.getElementsByClassName('active')
          current[0].className = current[0].className.replace(' active', '')
          this.className += ' active'
        })
      }
    }
  }
}
</script>
<style>
@import '../assets/css/style.css';
</style>