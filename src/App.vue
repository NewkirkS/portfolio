<template>
  <div id="app">
    <div>

    </div>
    <ProjectCard name="Test Name"
                 liveLink="link"
                 repoLink="link"
                 image="image"
                 description="This is an app"/>
  </div>
</template>

<script>
import ProjectCard from './components/ProjectCard.vue';

export default {
  name: 'App',
  components: {
    ProjectCard,
  },
  data() {
    return {
      projects: [
        {
          name: null,
          liveLink: null,
          repoLink: null,
          image: null,
          decription: null,
        },
        {
          name: null,
          liveLink: null,
          repoLink: null,
          image: null,
          decription: null,
        },
        {
          name: null,
          liveLink: null,
          repoLink: null,
          image: null,
          decription: null,
        },
      ],
    };
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
