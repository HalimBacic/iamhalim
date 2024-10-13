<template>
  <div id="app">
    <div class="section containerOne">
      <NavigationComponent></NavigationComponent>
      <InfoText></InfoText>
      <GraphComponent></GraphComponent>
    </div>
    <div class="section biography">
      <BiographyComponent></BiographyComponent>
    </div>
  </div>
</template>

<script>
import NavigationComponent from "./components/NavigationComponent.vue";
import InfoText from "./components/InfoText.vue";
import GraphComponent from "./components/Graph.vue";
import BiographyComponent from "./components/BiographyComponent.vue";

export default {
  name: "App",
  components: {
    NavigationComponent,
    InfoText,
    GraphComponent,
    BiographyComponent,
  },
};
</script>

<style>
body, #app {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.section
{
  height:100vh;
}
</style>
