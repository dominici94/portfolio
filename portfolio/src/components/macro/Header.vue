<template>
  <header class="header">
    <a href="/" class="header__link"
      ><img src="../../assets/img/logo.png" alt="logo" class="header__logo"
    /></a>

    <div class="header__heading">
      <h1 class="header__heading--main">Mattia Dominici</h1>
      <h2 class="header__heading--sub">front-end developer</h2>
    </div>

    <ul class="header__nav">
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Informazioni</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Esperienze</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Progetti</a>
      </li>
      <li class="header__nav--item">
        <a class="header__nav--link" href="#">Contatti</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>
