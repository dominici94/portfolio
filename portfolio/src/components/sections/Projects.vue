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
            <h4 class="projects__card__title">
              {{ project.title }}
            </h4>

            <p class="projects__card__description">
              {{ project.desc }}
            </p>

            <h4 class="projects__card__responsivness">
              Responsive:
              <svg v-if="project.reponsive" class="icon icon__success">
                <use
                  xlink:href="../../assets/img/sprite.svg#icon-checkmark"
                ></use>
              </svg>

              <svg v-else class="icon icon__fail">
                <use xlink:href="../../assets/img/sprite.svg#icon-cross"></use>
              </svg>
            </h4>

            <a class="projects__card__cta" :href="`${project.link}`"
              >Vai al progetto</a
            >
          </div>
        </li>
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
          desc: "Progetto svolto durante il corso di Boolean, consiste in una replica di Netflix, con funzionalità di ricerca di un film o serie tv tramite l'API di The Movie DB. Per lo sviluppo è stato adottato Vue.js come framework.",
          imgUrl: require("../../assets/img/preview_boolflix.png"),
          reponsive: false,
        },
        {
          title: "Omnifood",
          link: "https://course-omnifood.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sui fondamenti di HTML e CSS. Il progetto è incentrato sul layout del sito.",
          imgUrl: require("../../assets/img/preview_omnifood.png"),
          reponsive: true,
        },
        {
          title: "Natours",
          link: "https://css-course-natours.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sul CSS e Sass a livello avanzato. Il progetto è incentrato sul layout e gli effetti creati utilizzando esclusivamente il CSS.",
          imgUrl: require("../../assets/img/preview_natours.png"),
          reponsive: true,
        },
        {
          title: "Trillo",
          link: "https://css-course-flexbox-trillo.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sul CSS e Sass a livello avanzato. Il progetto è incentrato sull'ultilizzo del Flexbox nel CSS.",
          imgUrl: require("../../assets/img/preview_trillo.png"),
          reponsive: true,
        },
        {
          title: "Nexter",
          link: "https://css-course-grid-nexter.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sul CSS e Sass a livello avanzato. Il progetto è incentrato sull'utilizzo della proprietà Grid nel CSS.",
          imgUrl: require("../../assets/img/preview_nexter.png"),
          reponsive: true,
        },
        {
          title: "Pig game",
          link: "https://js-course-piggame.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sull'utilizzo di JavaScript. Il progetto è un semplice gioco nel quale un giocatore tira i dadi, se esce 1 tocca al giocatore avversario, se escono altri numeri, questi si possono accumulare all'attuale punteggio. Lo scopo finale è arrivare a 99 punti per primi",
          imgUrl: require("../../assets/img/preview_piggame.png"),
          reponsive: false,
        },
        {
          title: "Bankist",
          link: "https://js-course-bankist.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sull'utilizzo di JavaScript. Il progetto è incentrato sull'implementazione di features attraverso JavaScript.",
          imgUrl: require("../../assets/img/preview_bankist.png"),
          reponsive: false,
        },
        {
          title: "Mapty",
          link: "https://js-course-mapty.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sull'utilizzo di JavaScript. Il progetto è incentrato sull'utilizzo della geolocation API per rintracciare la posizione del client e utilizzarla per registrare attività di corsa o ciclismo.",
          imgUrl: require("../../assets/img/preview_mapty.png"),
          reponsive: false,
        },
        {
          title: "Forkify",
          link: "https://js-course-forkify.netlify.app",
          desc: "Progetto svolto seguendo il corso su Udemy di Jonas Schmedtmann sull'utilizzo di JavaScript. In questo progetto si può cercare ricette in base agli ingredienti, visualizzare le singole ricette e visualizzare la qunaittà di ingredienti in base alle porzioni richieste.",
          imgUrl: require("../../assets/img/preview_forkify.png"),
          reponsive: false,
        },
      ],
    };
  },
};
</script>

<style></style>
