<template>
  <section class="info">
    <div class="container">
      <div class="row">
        <div class="about">
          <h3 class="about__title">Informazioni</h3>
          <p class="about__text">
            Sono un junior front end developer con passione per la creazione di
            prodotti digitali coinvolgenti e intuitivi. Sono a conoscenza delle
            tecnologie web di bas HTML, CSS, JavaScript e framework come Vuejs.
            Ho anche una buona comprensione dei principi di design e
            dell'usabilità, che utilizzo per creare interfacce utente efficaci e
            gradevoli. Ho esperienza nella creazione di siti web responsive e
            ottimizzati per dispositivi mobili, nonché nella gestione di
            progetti in collaborazione con altri membri del team, come designer
            e sviluppatori back end. Sono sempre alla ricerca di nuove sfide e
            di migliorare le mie competenze, partecipando a conferenze e corsi
            di formazione. Sono in grado di lavorare bene sotto pressione e di
            rispettare le scadenze.Sono entusiasta di contribuire al successo
            dei progetti in cui lavoro.
          </p>
        </div>
        <figure class="img-container">
          <img
            class="img-photo"
            src="../../assets/img/img-profilo.jpg"
            alt="profile picture"
          />
        </figure>
      </div>

      <carousel :items-to-show="5" :wrapAround="true" :autoplay="2500">
        <slide
          v-for="slide in dataSlider"
          :key="slide"
          style="display: flex; flex-direction: column"
        >
          <figure style="width: 150px; height: 150px">
            <img :src="slide.imgUrl" :alt="slide.title" style="width: 100%" />
          </figure>
          <h3>{{ slide.title }}</h3>
        </slide>
      </carousel>
    </div>
  </section>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide } from "vue3-carousel";

export default {
  name: "Info",
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      dataSlider: [
        {
          title: "Html 5",
          imgUrl: require("../../assets/img/html5.png"),
        },
        {
          title: "Css 3",
          imgUrl: require("../../assets/img/css.png"),
        },
        {
          title: "Javascript",
          imgUrl: require("../../assets/img/js.png"),
        },
        {
          title: "Vue.js",
          imgUrl: require("../../assets/img/vuejs.png"),
        },
        {
          title: "Jquery",
          imgUrl: require("../../assets/img/jquery.png"),
        },
        {
          title: "Bootstrap",
          imgUrl: require("../../assets/img/bootstrap.png"),
        },
        {
          title: "Git",
          imgUrl: require("../../assets/img/git.png"),
        },
      ],
    };
  },
};
</script>
