<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <a class="navbar-brand" href="#"
      ><img src="../assets/icons/logo-1.svg" alt="" />
      <div class="brand-info">
        <span class="brand-name">zutterman</span>
        <span class="brand-description">Measure Tapes</span>
      </div>
    </a>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item" v-for="(link, index) in navbarLinks" :key="index">
          <a class="nav-link" :href="link.url">{{ link.name }}</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class Navbar extends Vue {
  navbarLinks = [
    { name: "ABOUT US", url: "#" },
    { name: "MODELS", url: "#" },
    { name: "GUARANTEE", url: "#" },
  ];
}
</script>

<style lang="scss">
@import "@/assets/scss/navbar.scss";
</style>
