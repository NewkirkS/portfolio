<template>
  <div id="app">
    <ProjectCard name="Test Name"
                 liveLink="link"
                 repoLink="link"
                 image="image"
                 description="This is an app"
        />
  </div>
</template>

<script>
import ProjectCard from './components/ProjectCard.vue';

export default {
  name: 'App',
  components: {
    ProjectCard,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
