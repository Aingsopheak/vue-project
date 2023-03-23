<template>
  <header class="header">
    <Navbar @toggle-menu-show="$emit('toggle-menu-show', $event)" />
    <Hero />
  </header>
</template>

<script>
import Navbar from "../Navbar.vue";
import Hero from "./Hero.vue";

export default {
  name: "Header",
  components: { Navbar, Hero },
  emits: ["toggle-menu-show"],
  methods: {
    clickHandler() {},
  },
};
</script>

<style lang="scss" scoped>
.header {
  background-image: url("../../assets/Untitled1.jpg");
  background-position: center;
  background-size: cover;

  @media (min-width: 768px) {
    background-image: url("../../assets/Untitled1.jpg");
    background-position: center;
    background-size: cover;
  }

  @media (min-width: 1205px) {
    background-image: url("../../assets/Untitled1.jpg");
    background-size: cover;
    background-position: center;
  }
}
</style>
