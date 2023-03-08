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
};
</script>

<style></style>
