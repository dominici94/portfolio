<template>
  <footer id="section--contacts" class="footer">
    <div class="container">
      <h3 class="heading heading-primary footer__heading">Contatti</h3>

      <div>
        <input v-model="emailData.name" type="text" required />
        <input v-model="emailData.email" type="email" required />
        <input v-model="emailData.bodyText" type="text" required />
        <button @click="SendEmail()">Send Email</button>

        {{ emailData }}
      </div>

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
  </footer>
</template>

<script>
import axios from "axios";

export default {
  name: "Footer",
  data() {
    return {
      emailData: {
        name: "",
        email: "",
        bodyText: "",
      },
    };
  },
  methods: {
    SendEmail() {
      axios
        .post(
          "https://khu61npt41.execute-api.us-east-2.amazonaws.com/prod/sendemail",
          this.emailData
        )
        .then((response) => {
          console.log(response);
          alert("Email Inviata");
        })
        .catch((err) => {
          console.log(err);
          alert("Errore email non inviata!");
        });
    },
  },
};
</script>
