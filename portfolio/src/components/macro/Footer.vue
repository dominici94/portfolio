<template>
  <div class="contacts">
    <ul class="contacts__links">
      <li>
        <a href="#"
          ><svg class="icon__mail">
            <use xlink:href="../../assets/img/sprite.svg#icon-gmail"></use></svg
        ></a>
      </li>
      <li>
        <a href="#"
          ><svg class="icon__linkedin">
            <use
              xlink:href="../../assets/img/sprite.svg#icon-linkedin"
            ></use></svg
        ></a>
      </li>
      <li>
        <a href="#"
          ><svg class="icon__github">
            <use
              xlink:href="../../assets/img/sprite.svg#icon-github"
            ></use></svg
        ></a>
      </li>
    </ul>

    <div class="contacts__copy">copyright 2023 Mattia Dominici</div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style>
.contacts {
  background-color: lightblue;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
