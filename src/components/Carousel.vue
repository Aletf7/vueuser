<template>
  <div class="row">
    <div class="col-sm">
      <carousel :data="data"></carousel>
    </div>
    <div class="col-sm mt-3 mt-sm-0">
      <carousel :data="data" indicator-type="disc"></carousel>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  data() {
    return {
      data: [
        <div class="example-slide">Slide 1</div>,
        <div class="example-slide">Slide 2</div>,
        <div class="example-slide">Slide 3</div>
      ]
    };
  }
};
</script>

<style>
.example-slide {
  align-items: center;
  background-color: #666;
  color: #999;
  display: flex;
  font-size: 1.5rem;
  justify-content: center;
  min-height: 10rem;
}
</style>
