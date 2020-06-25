<template>
  <div id="app">
    <div>
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand href="#">NA dos Santos Pinturas</b-navbar-brand>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <div>
              <span class="texts mr-2">47 98420-5285</span>
              <img src="../src/assets/whatsapp.svg" height="40" width="30" />
            </div>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <div>
      <b-carousel
        :interval="4000"
        controls
        indicators
        background="#ababab"
        img-width="1024"
        img-height="480"
        style="text-shadow: 1px 1px 2px #333;"
      >
        <b-carousel-slide caption="Blank Image 1" img-blank img-alt="Blank image">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
            a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
          </p>
        </b-carousel-slide>
        <b-carousel-slide caption="Blank Image 2" img-blank img-alt="Blank image">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
            a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
          </p>
        </b-carousel-slide>
        <b-carousel-slide caption="Blank Image 3" img-blank img-alt="Blank image">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse eros felis, tincidunt
            a tincidunt eget, convallis vel est. Ut pellentesque ut lacus vel interdum.
          </p>
        </b-carousel-slide>
      </b-carousel>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";

export default {
  name: "App"
};
</script>

<style scoped>
.texts {
  color: white;
  font-size: 20px;
  font-weight: bold;
}
</style>

