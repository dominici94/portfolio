<template>
  <section class="info">
    <div class="container">
      <div class="about">
        <div class="about__info">
          <h3 class="about__title heading heading-primary">Informazioni</h3>
          <p class="about__text">
            Sono un junior front-end developer con passione per la creazione di
            prodotti digitali coinvolgenti e intuitivi. Sono a conoscenza delle
            tecnologie web di base: HTML, CSS, JavaScript e framework come
            Vuejs. Ho anche una buona comprensione dei principi di design, che
            utilizzo per creare interfacce utente efficaci e gradevoli. Ho
            esperienza nella creazione di siti web responsive e ottimizzati per
            dispositivi mobili, nonché nella gestione di progetti in
            collaborazione con altri membri del team, come designer e
            sviluppatori back end. Sono sempre alla ricerca di nuove sfide e di
            migliorare le mie competenze, partecipando a conferenze e corsi di
            formazione. Sono in grado di lavorare bene sotto pressione e di
            rispettare le scadenze.
          </p>
        </div>
        <figure class="about__image-container">
          <img
            class="about__image-picture"
            src="../../assets/img/profilo.jpg"
            alt="profile picture"
          />
        </figure>
      </div>

      <div class="skills">
        <h3 class="skills__title heading heading-secondary">
          Tecnologie apprese
        </h3>

        <carousel :items-to-show="5" :wrapAround="true" :autoplay="2500">
          <slide
            v-for="slide in dataSlider"
            :key="slide.id"
            class="skills__slide"
          >
            <figure class="skills__img-container">
              <img
                class="skills__image"
                :src="slide.imgUrl"
                :alt="slide.title"
              />
              <figcaption class="skills__titte">{{ slide.title }}</figcaption>
            </figure>
          </slide>
        </carousel>
      </div>
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
          id: 1,
          title: "Html 5",
          imgUrl: require("../../assets/img/html5.png"),
        },
        {
          id: 2,
          title: "Css 3",
          imgUrl: require("../../assets/img/css.png"),
        },
        {
          id: 3,
          title: "Javascript",
          imgUrl: require("../../assets/img/js.png"),
        },
        {
          id: 4,
          title: "Sass",
          imgUrl: require("../../assets/img/sass.png"),
        },
        {
          id: 5,
          title: "Jquery",
          imgUrl: require("../../assets/img/jquery.png"),
        },
        {
          id: 6,
          title: "Vue.js",
          imgUrl: require("../../assets/img/vuejs.png"),
        },
        {
          id: 7,
          title: "Bootstrap",
          imgUrl: require("../../assets/img/bootstrap.png"),
        },
        {
          id: 8,
          title: "Git",
          imgUrl: require("../../assets/img/git.png"),
        },
        {
          id: 9,
          title: "Php",
          imgUrl: require("../../assets/img/php.png"),
        },
        {
          id: 10,
          title: "Laravel",
          imgUrl: require("../../assets/img/laravel.png"),
        },
      ],
    };
  },
};
</script>
