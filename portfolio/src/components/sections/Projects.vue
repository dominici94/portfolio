<template>
  <section class="projects">
    <div class="container">
      <h3 class="projects__heading heading heading-primary">Progetti</h3>

      <ul class="projects__container">
        <li
          v-for="project in dataProjects"
          :key="project.title"
          class="projects__card"
        >
          <div class="projects__card__side projects__card__side--front">
            <div class="projects__card__side--overlay"></div>
            <img
              :src="`${project.imgUrl}`"
              alt="preview image project"
              class="projects__card__preview"
            />
          </div>
          <div class="projects__card__side projects__card__side--back">
            <a class="projects__link" :href="`${project.link}`"
              >visita il progetto</a
            >
          </div>
        </li>
        <!-- 
        

        <li class="projects__item">
          <a href="https://js-course-forkify.netlify.app">Forkify</a>
        </li> 
        -->
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      dataProjects: [
        {
          title: "Boolflix",
          link: "https://boolflix-dominici.netlify.app",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Omnifood",
          link: "https://course-omnifood.netlify.app",
          desc: "prova",
          imgUrl: require("../../assets/img/preview_omnifood.png"),
          reponsive: false,
        },
        {
          title: "Natours",
          link: "https://css-course-natours.netlify.app",
          desc: "prova prova",
          imgUrl: require("../../assets/img/preview_natours.png"),
          reponsive: false,
        },
        {
          title: "Trillo",
          link: "https://css-course-flexbox-trillo.netlify.app",
          desc: "provaprovaprvoa",
          imgUrl: require("../../assets/img/preview_trillo.png"),
          reponsive: false,
        },
        {
          title: "Nexter",
          link: "https://css-course-grid-nexter.netlify.app",
          desc: "Prova",
          imgUrl: require("../../assets/img/preview_nexter.png"),
          reponsive: false,
        },
        {
          title: "Pig game",
          link: "https://js-course-piggame.netlify.app",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_piggame.png"),
          reponsive: false,
        },
        {
          title: "Bankist",
          link: "https://js-course-bankist.netlify.app",
          desc: "Proiva",
          imgUrl: require("../../assets/img/preview_bankist.png"),
          reponsive: false,
        },
        {
          title: "Mapty",
          link: "https://js-course-mapty.netlify.app",
          desc: "prova prova",
          imgUrl: require("../../assets/img/preview_mapty.png"),
          reponsive: false,
        },
        {
          title: "Forkify",
          link: "https://js-course-forkify.netlify.app",
          desc: "provonma",
          imgUrl: require("../../assets/img/preview_forkify.png"),
          reponsive: false,
        },
      ],
    };
  },
};
</script>

<style></style>
