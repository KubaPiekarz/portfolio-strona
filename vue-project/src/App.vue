<template>
  <div id="app">
    <Introduction />
    <WhoAmI />
    <Experience />
    <TechnologyStack />
    <Projects />
    <Contact />
  </div>
</template>

<script setup>
import Introduction from './components/Introduction.vue';
import WhoAmI from './components/WhoAmI.vue';
import Experience from './components/Experience.vue';
import TechnologyStack from './components/TechnologyStack.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
</script>

<style>
body {
  font-family: 'Roboto';
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  width: 100%;
}
</style>