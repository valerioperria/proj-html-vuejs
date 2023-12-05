<script>
import AppHeader from "./components/AppHeader.vue";
import Section1 from "./components/Section1.vue";
import Section2 from "./components/Section2.vue";
export default {
  components: { AppHeader, Section1, Section2 },
}; 
</script>

<template>
  <AppHeader />
  <Section1 />
  <Section2 />
</template>

<style lang="scss">
@use "./style/General.scss";
@import "@fortawesome/fontawesome-free/css/all.css";
</style>