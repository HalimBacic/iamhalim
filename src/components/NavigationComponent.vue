<template>
  <div class="navigation">
    <div class="btn" @click="scrollTo('cvId')">About me</div>
    <div class="btn" @click="scrollTo('')">Contacts</div>
  </div>
</template>

<script scoped>
export default {
  name: "navigationComponent",
  methods: {
    scrollTo(sectionId) {
      const section = document.getElementById(sectionId);
      if (section) {
        section.scrollIntoView({ behavior: "smooth" });
      }
      else
        console.warn(`Element with id '${sectionId}' not found.`);
    },
  },
};
</script>

<style>
.navigation {
  display: flex;
  flex-direction: row;
  width: 30%;
  justify-content: space-around;
  font-family: "Play", sans-serif;
  font-weight: 600;
  top: 10vh;
  position: relative;
  height: 10%;
}

.btn:hover {
  cursor: pointer;
}
</style>
