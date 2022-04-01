<template>
  <div class="home">
    <main-content></main-content>
    <Footer></Footer>
  </div>
</template>

<script lang="ts">
import Footer from "@/components/Footer.vue";
import MainContent from "@/components/MainContent.vue";
import { Options, Vue } from "vue-class-component";

@Options({
  components: { "main-content": MainContent, Footer: Footer },
})
export default class HomeView extends Vue {}
</script>

<style lang="scss" scoped></style>
