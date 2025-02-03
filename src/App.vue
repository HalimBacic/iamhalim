<template>
  <div id="app">
    <div class="section containerOne">
      <div class="containerTwo">
          <NavigationComponent></NavigationComponent>
          <GraphComponent></GraphComponent>
      </div>
      <InfoText></InfoText>
    </div>
    <div class="cv" id="cvId">
      <CvComponent></CvComponent>
    </div>
  </div>
</template>

<script>
import InfoText from "./components/InfoText.vue";
import GraphComponent from "./components/Graph.vue";
import NavigationComponent from './components/NavigationComponent.vue';
import CvComponent from "./components/CvComponent.vue";

export default {
  name: "App",
  components: {
    InfoText,
    GraphComponent,
    NavigationComponent,
    CvComponent
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
  height: 100vh;
}

.cv
{
  height: 100%;
}

.containerTwo
{
  display: flex;
  height: 100vh;
}

.ContainerOne
{
  height:100vh;
}
</style>
