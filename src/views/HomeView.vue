<template>
  <div class="home">
    <Navbar></Navbar>
    <main-content></main-content>
    <Footer></Footer>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Navbar from "@/components/Navbar.vue";
import MainContent from "@/components/MainContent.vue";
import Footer from "@/components/Footer.vue";

@Options({
  components: { "main-content": MainContent, Footer: Footer, Navbar: Navbar },
})
export default class HomeView extends Vue {}
</script>

<style lang="scss" scoped></style>
