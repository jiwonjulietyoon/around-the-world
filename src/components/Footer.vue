<template>
  <footer>
    <small>Copyright &copy; {{currentYear}} JiwonJulietYoon. All Rights Reserved</small>
  </footer>
</template>


<script>
export default {
  name: "Footer",
  data: () => ({
    currentYear: 0
  }),
  methods: {
    getCurrentYear() {
      let d = new Date();
      this.currentYear = d.getFullYear();
    }
  },
  mounted() {
    this.getCurrentYear();
  }
}
</script>


<style lang="scss" scoped>
@import "@/css/style.scss";

footer {
  height: 100px;
  background: $bg-dk-gr;
  text-align: center;
  color: white;
  letter-spacing: 1px;
}
</style>