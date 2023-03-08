<template>
  <div class="footer">
    <div class="container">
      <h3 class="heading heading-primary footer__heading">Contatti</h3>
      <div class="contacts">
        <ul class="contacts__list">
          <li class="contacts__item">
            <a class="contacts__link" href="mailto:mattiadominici94@gmail.com"
              ><svg class="icon icon__mail">
                <use
                  xlink:href="../../assets/img/sprite.svg#icon-gmail"
                ></use></svg
            ></a>
          </li>
          <li class="contacts__item">
            <a
              class="contacts__link"
              href="https://www.linkedin.com/in/mattia-dominici-b2a923232/"
              ><svg class="icon icon__linkedin">
                <use
                  xlink:href="../../assets/img/sprite.svg#icon-linkedin"
                ></use></svg
            ></a>
          </li>
          <li class="contacts__item">
            <a class="contacts__link" href="https://github.com/dominici94"
              ><svg class="icon icon__github">
                <use
                  xlink:href="../../assets/img/sprite.svg#icon-github"
                ></use></svg
            ></a>
          </li>
        </ul>

        <div class="contacts__copy">&copy; Mattia Dominici - 2023</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>
