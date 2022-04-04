<template>
  <main>
    <div class="section-one-container">
      <p class="section-one-title">Measuring Everything</p>
      <img
        src="../assets/images/tapes-1.png"
        alt="Fita métrica"
        class="section-one-image"
      />
    </div>
    <div class="section-two-container">
      <div class="text-container">
        <p class="section-two-title">We are Leader in Measure Tapes</p>
        <span class="section-two-description"
          >There are 5x the circumference of planet earth in metric tapes.</span
        >
      </div>
      <img
        src="../assets/images/tape-2.png"
        alt="Fita métrica"
        class="section-two-image"
      />
    </div>
  </main>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class MainContent extends Vue {}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/main.scss";
</style>
