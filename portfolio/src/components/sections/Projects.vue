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
        <!-- <a
            class="projects__link"
            href="https://boolflix-dominici.netlify.app"
          >
            <img :src="`${project.imgUrl}`" alt="preview image project" />
          </a> -->
        <!-- <li class="projects__item">
          <a href="https://course-omnifood.netlify.app">Omnifood</a>
        </li>
        <li class="projects__item">
          <a href="https://css-course-natours.netlify.app">Natours</a>
        </li>
        <li class="projects__item">
          <a href="https://css-course-flexbox-trillo.netlify.app">Trillo</a>
        </li>
        <li class="projects__item">
          <a href="https://css-course-grid-nexter.netlify.app">Nexter</a>
        </li>
        <li class="projects__item">
          <a href="https://js-course-piggame.netlify.app">Pig game</a>
        </li>
        <li class="projects__item">
          <a href="https://js-course-bankist.netlify.app">Bankist</a>
        </li>
        <li class="projects__item">
          <a href="https://js-course-mapty.netlify.app">Mapty</a>
        </li>
        <li class="projects__item">
          <a href="https://js-course-forkify.netlify.app">Forkify</a>
        </li> -->
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
          link: "https://boolflix-dominici.netlify.app",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_omnifood.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Boolflix",
          desc: "Replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
      ],
    };
  },
};
</script>

<style></style>
