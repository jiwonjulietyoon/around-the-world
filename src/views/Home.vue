<template>
  <div id="wrap">
    
    <!-- INTRO -->
    <section class="intro">
      <Intro />
    </section>

    <!-- GALLERY -->
    <section class="gallery">
      <Gallery />
    </section>

    <!-- MAP -->
    <section class="map">
      <Map />
    </section>

  </div>
</template>

<script>
import Intro from "@/components/IntroSection/Intro";
import Gallery from "@/components/GallerySection/Gallery";
import Map from "@/components/MapSection/Map";

export default {
  name: "Home",
  components: {
    Intro,
    Gallery,
    Map
  },
};
</script>


<style lang="scss" scoped>
@import "@/css/style.scss";

section {
  width: 100%;
  height: 100vh;
  overflow-y: hidden;
  overflow-x: auto;
  position: relative;
}

section.intro, section.map {
  background-color: $bg-lt;
}

</style>