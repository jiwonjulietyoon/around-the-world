<template>
  <v-app id="Vapp">
    <router-view />
    <Footer />
  </v-app>
</template>

<script>
import Footer from "@/components/Footer";

export default {
  name: 'App',
  components: {
    Footer,
  },
  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
@import "./css/reset.css";
@import "@/css/style.scss";


</style>