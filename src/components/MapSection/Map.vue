<template>
  <div>
    <h2 class="section-title">World Map</h2>
    <div class="world-map">
      <img src="~@/assets/world_map.svg" alt="World Map">
      <div class="locations">
        
      </div>
    </div>
    
  </div>
</template>

<script>

export default {
  name: "Map",
  components: {

  },
};
</script>


<style lang="scss" scoped>
@import "@/css/style.scss";

.world-map {
  width: 90%;
  max-width: 1000px;
  @include md-down {width: 95%;}
  @include sm-down {width: 100%;}
  margin: 0 auto;
  height: auto;
  border: 1px solid hotpink;
  position: relative;
  & > img {
    width: 100%;
  }
}

</style>