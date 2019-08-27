<template>
  <div class="intro-container">
    <div class="globe-outer">
      <div class="globe">
        
        <!-- Globe Inner -->
        <div class="band b1"></div>
        <div class="band b2"></div>
        <div class="band b3"></div>
        <div class="title">
          <div>
            <span class="a">Around</span>
          </div>
          <div>
            <span class="t">the </span>
            <span class="w">World</span>
          </div>
        </div>

        <!-- Globe Outer -->
        <div class="outer-band ">

        </div>
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
  @include sm-down {
    width: 42%;
    padding-top: 42%;
  }
  @include xs-down {
    width: 55%;
    padding-top: 55%;
  }
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
    border-style: solid;
    &.b1 {
      width: calc(100% - 10px);
      height: calc(100% - 10px);
      border-width: 3px;
      border-color: $blue-accent $blue-accent $blue-accent $transparent;
    }
    &.b2 {
      width: calc(100% - 22px);
      height: calc(100% - 22px);
      border-width: 2px;
      border-color: $blue-accent-lt $blue-accent-lt $blue-accent-lt $transparent;
    }
    &.b3 {
      width: calc(100% - 30px);
      height: calc(100% - 30px);
      border-width: 2.5px;
      border-color: $blue-accent $blue-accent $blue-accent $transparent;
    }
  }
  & > .title {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%) rotate(-10deg);
    .a {
      font-size: 2em;
      @include sm-down {font-size: 1.6em;}
    }
    .t {
      font-size: 1.2em;
      @include sm-down {font-size: 1em;}
    }
    .w {
      font-size: 1.7em;
      @include sm-down {font-size: 1.3em;}
    }
  }
}


</style>