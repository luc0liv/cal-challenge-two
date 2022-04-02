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
@import "@/assets/scss/main.scss";
.navbar {
  display: flex;
  justify-content: flex-end;
}
.navbar-light {
  padding: 1rem 3rem;
  .navbar-toggler {
    border: 0;
  }
  .navbar-toggler:focus {
    box-shadow: none;
  }
  .navbar-toggler-icon {
    background-image: url("@/assets/icons/menu-icon.svg");
    width: 6px;
  }

  .navbar-brand {
    display: flex;
    align-items: flex-end;
    column-gap: 2rem;

    .brand-info {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-items: center;

      @media screen and (max-width: 992px) {
        display: none;
      }
    }
    img {
      height: 70px;
      width: 70px;
    }
  }

  .navbar-nav {
    margin-left: auto;
    column-gap: 4rem;

    .nav-item {
      .nav-link {
        color: $primary-text-color;
        font-weight: lighter;
        letter-spacing: 5.4px;
      }
    }
  }

  .brand-name {
    color: $primary-text-color;
    font-weight: bold;
    font-size: 41.2px;
    margin-bottom: -10px;
  }
  .brand-description {
    color: $primary-text-color;
    font-weight: lighter;
    font-size: 1rem;
    letter-spacing: 5.4px;
  }
}
</style>
