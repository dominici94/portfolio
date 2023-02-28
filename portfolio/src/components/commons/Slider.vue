<template>
  <carousel :items-to-show="1.5">
    <slide v-for="slide in dataSlider" :key="slide">
      <h3>{{ slide.title }}</h3>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
  name: "Slider",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data() {
    return {
      dataSlider: [
        {
          title: "Html 5",
          // imgUrl: "",
        },
        {
          title: "Css 3",
        },
        {
          title: "Javascript",
        },
      ],
    };
  },
};
</script>
