<template>
  <div class="navigation">
    <div class="leftSide">
      <div class="myBtn">Bio</div>
      <div class="myBtn">Projects</div>
      <div class="myBtn">TechStack</div>
    </div>
    <div class="rightSide">
        <v-icon name="si-gmail" class="icon" @click="GoToGmail"/>
        <v-icon name="bi-github" class="icon" @click="OpenGitHub"/>
        <v-icon name="bi-linkedin" class="icon" @click="OpenLinkedId"/>
    </div>
  </div>
</template>

<script>
import { SiGmail, BiGithub, BiLinkedin } from 'oh-vue-icons/icons';
import { addIcons, OhVueIcon } from 'oh-vue-icons';

addIcons(SiGmail, BiGithub, BiLinkedin);
export default {
  name: "NavigationComponent",
  components:
  {
    "v-icon":OhVueIcon
  },
  methods:
  {
    GoToGmail()
    {window.open("mailto:bacich95@gmail.com");},
    OpenGitHub()
    {window.open("https://github.com/HalimBacic", "_blank");},
    OpenLinkedId()
    {window.open("www.linkedin.com/in/halimbacic", "_blank");}
  }
};
</script>

<style scoped>
.navigation {
  font-family: "Nunito", sans-serif;
  font-weight: 800;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
}

.leftSide
{
    display: flex;
    justify-content: flex-start;
    padding-right: 2vw;
    flex-direction: row;
    width: 60%;
    float: left;
}

.rightSide
{
    float: right;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    width: 25%;
}

.icon {
  color: #d62246;
  scale: 1.5;
  height: 40px;
}

.icon:hover
{
    cursor: pointer;
    animation: "float";
}

.myBtn {
  width: 15%;
  font-size: 3vh;
  color: #0E7C7B;
  height: 40px;
}

.myBtn:hover {
  cursor: pointer;
  color:#d62246;
}
</style>
