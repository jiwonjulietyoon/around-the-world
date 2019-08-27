<template>
  <div class="intro-container">
    <div class="globe-outer">
      <div class="globe">
        <div class="band b1"></div>
        <div class="band b2"></div>
        <div class="band b3"></div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "Intro",
  components: {

  },
};
</script>


<style lang="scss" scoped>
@import "@/css/style.scss";

.intro-container {
  width: 100%;
  min-width: 350px;
  max-width: 900px;
  height: 100%;
  min-height: 400px;
  border: 1px solid pink;
  @include center-item;
}
.globe-outer {
  width: 35%;
  padding-top: 35%;
  @include center-item;
}
.globe {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  @include center-item;
  border: 12px ridge $bg-dk-bl;
  & > .band {
    border-radius: 50%;
    @include center-item;
    &.b1 {
      width: calc(100% - 10px);
      height: calc(100% - 10px);
      border-width: 5px;
      border-style: solid;
      border-color: $blue-accent $blue-accent $blue-accent $transparent;
    }
  }
}


</style>