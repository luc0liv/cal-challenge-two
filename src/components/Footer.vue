<template>
  <div class="footer-container">
    <p>oie</p>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class Footer extends Vue {}
</script>

<style lang="scss" scoped>
.footer-container {
  background-color: #e9e9e9;
}
</style>
