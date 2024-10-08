<template>
  <div class="containerOne">
    <NavigationComponent></NavigationComponent>
    <InfoText></InfoText>
    <GraphComponent></GraphComponent>
  </div>
</template>

<script>
import NavigationComponent from "./components/NavigationComponent.vue";
import InfoText from "./components/InfoText.vue";
import GraphComponent from "./components/Graph.vue"

export default {
  name: "App",
  components: {
    NavigationComponent,
    InfoText,
    GraphComponent
  },
};
</script>

<style>
body {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
