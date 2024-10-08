<template>
  <div class="container">
    <div class="text1">IamHalim</div>
    <div class="text2">&lt;Software Engineer\&gt; </div>
  </div>
</template>

<script>
export default {
  name: "InfoText",
};
</script>

<style scoped>
.container{
    position: absolute;
    top:48vh;
    left:25vh;
    border-bottom: #D62246;
}
.text1 {
  font-family: "Passion One", sans-serif;
  font-weight: 400;
  color: #0E7C7B;
  position: relative;
  top: 5vh;
  left: 3vw;
  font-size: 165px;
  -webkit-text-stroke: 2px #D62246;
}
.text2 {
  font-family: "Play", sans-serif;
  font-weight: 600;
  position: relative;
  left: 5vw;
  font-size: 49px;
}
</style>
