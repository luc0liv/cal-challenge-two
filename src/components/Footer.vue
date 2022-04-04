<template>
  <footer class="footer-container">
    <div class="social-wrapper">
      <p class="social-title">Follow us</p>
      <div class="social-icons">
        <a
          v-for="(icon, index) in socialIcons"
          :key="index"
          :href="icon.url"
          target="_blank"
          rel="noopener noreferrer"
          ><img
            class="social-icon"
            :src="require(`../assets/icons/${icon.iconPath}`)"
            alt=""
        /></a>
      </div>
    </div>
    <div class="contact-wrapper">
      <p class="contact-title">Contact</p>
      <p class="contact-address">
        2490 Leisure Lane <br />
        San Luis Obispo <br />California
      </p>
    </div>
  </footer>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {},
})
export default class Footer extends Vue {
  socialIcons = [
    { iconPath: "youtube-icon.svg", url: "https://www.youtube.com/" },
    { iconPath: "facebook-icon.svg", url: "https://www.facebook.com/" },
    { iconPath: "twitter-icon.svg", url: "https://www.twitter.com/" },
  ];
}
</script>

<style lang="scss">
@import "@/assets/scss/footer.scss";
</style>
