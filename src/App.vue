<template>
  <div id="app">
    <div style="font-size: 20px">
      <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
        <b-navbar-brand href="#">
          <h3>NA dos Santos Pinturas</h3>
        </b-navbar-brand>
        <b-navbar-nav class="ml-auto">
          <div class="mr-2">
            <a href="tel:47 98420-5285">
              <img class="mr-2" src="../src/assets/whatsapp.svg" height="20" width="20" />
              <span class="texts mr-2">47 98420-5285</span>
            </a>
          </div>
          <div class="mr-2">
            <a href="https://www.facebook.com/www.n.ados.santos.com.br">
              <img class="mr-2" src="../src/assets/facebook.svg" height="20" width="20" />
              <span class="texts mr-2">Nadossantos Pinturas</span>
            </a>
          </div>
          <div class="mr-2">
            <a href="https://www.instagram.com/n.a.dos.santos_pinturas/">
              <img class="mr-2" src="../src/assets/instagram.svg" height="20" width="20" />
              <span class="texts mr-2">n.a.dos.santos_pinturas</span>
            </a>
          </div>
          <div>
            <a href="mailto:n.a.dos.santos@outlook.com?subject=Contato">
              <b-icon class="mr-2" style="color: white;" font-scale="1" icon="envelope" />
              <span class="texts mr-2">n.a.dos.santos@outlook.com</span>
            </a>
          </div>
        </b-navbar-nav>
      </b-navbar>
    </div>
    <div class="mt-1">
      <b-carousel
        :interval="4000"
        controls
        indicators
        background="#ababab"
        style="text-shadow: 1px 1px 2px #333;"
      >
        <b-carousel-slide v-for="(path, i) in carouselImages" :key="i">
          <template v-slot:img>
            <img class="w-100" height="800" :src="path" />
          </template>
        </b-carousel-slide>
      </b-carousel>
    </div>
    <div class="mt-2">
      <b-row>
        <b-col cols="12" md="8">
          <div class="w-100 mt-1" style="height: 500px; background-color: #eb3434;">
            <h1 class="text-center">ME DIZ ALGO PRA ESCREVER AQUI</h1>
          </div>
        </b-col>
        <b-col>
          <facebook />
        </b-col>
      </b-row>
    </div>
    <div class="w-100 mt-1" style="height: 500px; background-color: #2125a3;">
      <h1 class="text-center">ME DIZ OUTRA COISA PRA COLOCAR NESSE BLOCK</h1>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import carouselImages from "./assets/carousel-images";
import Facebook from "./components/Facebook";

export default {
  name: "App",
  components: {
    Facebook
  },
  data() {
    return {
      carouselImages: carouselImages
    };
  }
};
</script>

<style scoped>
.texts {
  color: white;
  font-size: 20px;
  font-weight: bold;
}
</style>

