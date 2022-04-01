<template>
  <div class="section-one-container">
    <p class="section-one-text">Measuring Everything</p>
    <img
      src="../assets/images/tapes-1.png"
      alt="Fita métrica"
      class="section-one-image"
    />
  </div>
  <div class="section-two-container">
    <div class="text-container">
      <p class="section-two-text">We are Leader in Measure Tapes</p>
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
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class MainContent extends Vue {}
</script>

<style lang="scss" scoped>
$navbar-height: 10vh;
$footer-height: 10vh;
.section-one-container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  background-color: #e9e9e9;
  height: 100vh;
  width: 100%;

  .section-one-image {
    mix-blend-mode: multiply;
    width: 40%;
  }

  .section-one-text {
    color: #716565;
    font-weight: bold;
    font-size: 82.2px;
    width: 30%;
  }
}

.section-two-container {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  background-color: #506fa9;
  height: calc(100vh - 10px);

  .section-two-image {
    mix-blend-mode: multiply;
    width: 60%;
  }

  .text-container {
    display: flex;
    flex-direction: column;
    padding-left: 100px;
    .section-two-text {
      color: #ffffff;
      font-weight: bold;
      font-size: 69.2px;
      line-height: 81.09px;
      margin-bottom: 10px;
    }
    .section-two-description {
      color: #ffffff;
      font-weight: lighter;
      font-size: 48.2px;
      line-height: 56.48px;
    }
  }
}
</style>
