<template>
  <div>
    <div class="navcontainer">
      <button @click="changeComponent('AboutContainer')">
        About Me
      </button>
      <button @click="changeComponent('EducationContainer')">
        Education
      </button>
      <button @click="changeComponent('ExperienceContainer')">
        Experience
      </button>
    </div>
    <div class="cvcontainer">
      <transition name="slide" mode="out-in">
        <component :is="activeComponent" :key="activeComponent" />
      </transition>
    </div>
  </div>
</template>

<script>
import AboutContainer from "./AboutContainer.vue";
import EducationContainer from "./EducationContainer.vue";
import ExperienceContainer from "./ExperienceContainer.vue";

export default {
  name: "CvComponent",
  components: {
    AboutContainer,
    EducationContainer,
    ExperienceContainer,
  },
  data() {
    return {
      activeComponent: "AboutContainer",
    };
  },
  methods: {
    changeComponent(componentName) {
      this.activeComponent = componentName;
    }
  }
};
</script>

<style scoped>
div{
  height:70%;
}

.content {
  position: relative;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
}

.cvcontainer {
  display: flex;
  flex-direction: row;
  height: 90vh;
}

.navcontainer {
  display: flex;
  flex-direction: row;
  width: 30%;
  justify-content: space-around;
  font-family: "Play", sans-serif;
  font-weight: 600;
  position: relative;
  height: 10%;
}

button {
  padding: 10px 20px;
  color: black;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  font-family: "Play", sans-serif;
  font-weight: 600;
  color: #2c3e50;
  font-size:20px;
  background-color: transparent;
  padding-bottom: 20px;
}

.slide-enter-active {
  animation: slide-in 0.5s ease-out forwards;
}

.slide-leave-active {
  animation: slide-out 0.5s ease-in forwards;
}

@keyframes slide-in {
  from {
    transform: translateX(100%);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

@keyframes slide-out {
  from {
    transform: translateX(0);
    opacity: 1;
  }
  to {
    transform: translateX(-100%);
    opacity: 0;
  }
}
</style>
