<template>
  <div id="main">
    <header class="header">
      <Logo />
      <NavList v-bind:navs="navs" />
    </header>

    <section class="banner">
      <BannerSvg />
      <MainImgs />
    </section>
  </div>
</template>

<script>
import NavList from "@/components/NavList/NavList";
import Logo from "@/components/Logo/Logo";
import BannerSvg from "@/components/BannerSvg/BannerSvg";
import MainImgs from "@/components/MainImgs/MainImgs";

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
    MainImgs,
  }
};
</script>

<style lang="scss">
  @import './Main.module.scss';
</style>