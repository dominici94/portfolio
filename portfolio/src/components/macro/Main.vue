<template>
  <main class="main">
    <Info />
    <Experiences />
    <Projects />
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
  mounted() {
    const allReveals = document.querySelectorAll(".reveal");

    const revealExperience = function (entries, observer) {
      const [entry] = entries;

      if (!entry.isIntersecting) return;
      console.log(entry);
      entry.target.classList.add("active");
      observer.unobserve(entry.target);
    };

    const revealObserver = new IntersectionObserver(revealExperience, {
      root: null,
      threshold: 0,
      rootMargin: "25%",
    });

    allReveals.forEach(function (card) {
      revealObserver.observe(card);
    });
  },
};
</script>
