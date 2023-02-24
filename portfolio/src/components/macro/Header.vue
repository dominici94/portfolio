<template>
  <header class="header">
    <a href="/" class="header__link"
      ><img src="../../assets/img/logo.png" alt="logo" class="header__logo"
    /></a>

    <div class="header__heading">
      <h1 class="header__heading--main">Mattia Dominici</h1>
      <h2 class="header__heading--sub">web developer</h2>
    </div>

    <ul class="header__nav">
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">About me</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Experience/Skills</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Works/Projects</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Contact</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style></style>
