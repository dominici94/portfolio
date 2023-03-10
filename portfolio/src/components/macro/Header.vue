<template>
  <header class="header">
    <a href="/" class="header__link"
      ><img src="../../assets/img/logo.png" alt="logo" class="header__logo"
    /></a>

    <div class="header__heading heading">
      <h1 class="header__heading--main">Mattia Dominici</h1>
      <h2 class="header__heading--sub">front-end developer</h2>
    </div>

    <ul class="header__nav">
      <li class="header__nav--item">
        <a class="header__nav--link" href="#section--info">Informazioni</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#section--experiences">Esperienze</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#section--projects">Progetti</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#section--contacts">Contatti</a>
      </li>
    </ul>

    <input type="checkbox" class="mobile__checkbox hidden" id="navi-toggle" />

    <label for="navi-toggle" class="mobile__button">
      <span class="mobile__icon">&nbsp;</span>
    </label>

    <ul class="mobile__nav">
      <li class="mobile__nav--item">
        <a class="mobile__nav--link" href="#section--info">Informazioni</a>
      </li>
      <li class="mobile__nav--item">
        <a class="mobile__nav--link" href="#section--experiences">Esperienze</a>
      </li>
      <li class="mobile__nav--item">
        <a class="mobile__nav--link" href="#section--projects">Progetti</a>
      </li>
      <li class="mobile__nav--item">
        <a class="mobile__nav--link" href="#section--contacts">Contatti</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
  mounted() {
    document
      .querySelector(".header__nav")
      .addEventListener("click", function (e) {
        e.preventDefault();

        if (e.target.classList.contains("header__nav--link")) {
          const id = e.target.getAttribute("href");
          document.querySelector(id).scrollIntoView({ behavior: "smooth" });
        }
      });

    const toggleNavigation = document.getElementById("navi-toggle");

    document
      .querySelector(".mobile__nav")
      .addEventListener("click", function (e) {
        e.preventDefault();

        if (e.target.classList.contains("mobile__nav--link")) {
          const id = e.target.getAttribute("href");
          document.querySelector(id).scrollIntoView({ behavior: "smooth" });
          toggleNavigation.checked = !toggleNavigation.checked;
        }
      });
  },
};
</script>
