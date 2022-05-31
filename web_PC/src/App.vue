<script setup>
import HeadMenu from "@/components/HeadMenu.vue";
import Banners from "@/components/Banners.vue";
import About from "@/components/About.vue";
import Solutions from "@/components/Solutions.vue";
import Careers from "@/components/Careers.vue";
import Gallery from "@/components/Gallery.vue";
import Contact from "@/components/Contact.vue";
import FootLogo from "@/components/FootLogo.vue";
</script>

<template>
  <HeadMenu />
  <main>
    <Banners />
    <About />
    <Solutions />
    <Careers />
    <Gallery />
    <Contact />
    <FootLogo />
  </main>
</template>

<style>
@import "@/assets/css/base.css";
main {
  height: calc(100vh - 50px);
  overflow-y: scroll;
}
</style>
