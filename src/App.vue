<script>
import AppFooter from "./components/AppFooter.vue";
import AppHeader from "./components/AppHeader.vue";
import Section1 from "./components/Section1.vue";
import Section2 from "./components/Section2.vue";
import Section3 from "./components/Section3.vue";
import Section4 from "./components/Section4.vue";
import Section5 from "./components/Section5.vue";
import Section6 from "./components/Section6.vue";
import Section7 from "./components/Section7.vue";
export default {
  components: { AppHeader, Section1, Section2, Section3, Section4, Section5, Section6, Section7, AppFooter },
}; 
</script>

<template>
  <AppHeader />
  <Section1 />
  <Section2 />
  <Section3 />
  <Section4 />
  <Section5 />
  <Section6 />
  <Section7 />
  <AppFooter />
</template>

<style lang="scss">
@use "./style/General.scss";
@import "@fortawesome/fontawesome-free/css/all.css";
</style>