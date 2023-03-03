<template>
  <div class="contacts">
    <ul class="contacts__links">
      <li>
        <a href="#">github icon</a>
      </li>
      <li>
        <a href="#">linkedin icon</a>
      </li>
      <li>
        <a href="#">gmail icon</a>
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
