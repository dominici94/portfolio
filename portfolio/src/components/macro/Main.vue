<template>
  <main class="main">
    <Info />
    <Experiences />
    <Projects />
    <!-- <h2 class="progetti">Progetti</h2>
    <div class="progetti"></div> -->
    <!-- <ul>
      <li><a href="https://boolflix-dominici.netlify.app">Boolflix</a></li>
      <li><a href="https://course-omnifood.netlify.app">Omnifood</a></li>
      <li><a href="https://css-course-natours.netlify.app">Natours</a></li>
      <li>
        <a href="https://css-course-flexbox-trillo.netlify.app">Trillo</a>
      </li>
      <li>
        <a href="https://css-course-grid-nexter.netlify.app">Nexter</a>
      </li>
      <li><a href="https://js-course-piggame.netlify.app">Pig game</a></li>
      <li><a href="https://js-course-bankist.netlify.app">Bankist</a></li>
      <li><a href="https://js-course-mapty.netlify.app">Mapty</a></li>
      <li><a href="https://js-course-forkify.netlify.app">Forkify</a></li>
    </ul> -->
  </main>
</template>

<script>
import Info from "../sections/Info.vue";
import Experiences from "../sections/Experiences.vue";
import Projects from "../sections/Projects.vue";

export default {
  name: "Main",
  components: {
    Info,
    Experiences,
    Projects,
  },
};
</script>

<style></style>
