<template>
  <div id="main">
    <header class="header">
      <Logo />
      <NavList v-bind:navs="navs" />
    </header>

    <section class="banner">
      <BannerSvg />
      <BannerImgs />
      <BannerLogo />
      <BannerSideLogos />
    </section>

    <footer class="footer">
      <Footer />
    </footer>
  </div>
</template>

<script>
import NavList from "@/components/NavList/NavList";
import Logo from "@/components/Logo/Logo";
import BannerSvg from "@/components/BannerSvg/BannerSvg";
import BannerImgs from "@/components/BannerImgs/BannerImgs";
import BannerLogo from "@/components/BannerLogo/BannerLogo";
import BannerSideLogos from "@/components/BannerSideLogos/BannerSideLogos";
import Footer from "@/components/Footer/Footer";

export default {
  name: "Main",
  data() {
    return {
      navs: [
        { id: 1, title: "Commercial" },
        { id: 2, title: "Editorial" },
        { id: 3, title: "Reportage" },
        { id: 3, title: "Meet Me" }
      ]
    };
  },
  components: {
    Logo,
    NavList,
    BannerSvg,
    BannerImgs,
    BannerLogo,
    BannerSideLogos,
    Footer,
  }
};
</script>

<style lang="scss">
  @import './Main.module.scss';
</style>