<template>
  <div id="app">
    <div class='project-container'>
      <ProjectCard v-for="(project) in projects"
              :key="project.id"
              :name="project.name"
              :liveLink="project.liveLink"
              :repoLink="project.repoLink"
              :image="project.image"
              :description="project.description"/>
    </div>
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
          id: 1,
          name: 'Project One',
          liveLink: 'https://github.com/NewkirkS/portfolio',
          repoLink: 'https://github.com/NewkirkS/portfolio',
          image: 'logo.png',
          description: 'This is the description of the application. It has multiple features.',
        },
        {
          id: 2,
          name: 'Project Two',
          liveLink: 'https://github.com/NewkirkS/portfolio',
          repoLink: 'https://github.com/NewkirkS/portfolio',
          image: 'logo.png',
          description: 'This is the description of the application. It has multiple features.',
        },
        {
          id: 3,
          name: 'Project Three',
          liveLink: 'https://github.com/NewkirkS/portfolio',
          repoLink: 'https://github.com/NewkirkS/portfolio',
          image: 'logo.png',
          description: 'This is the description of the application. It has multiple features.',
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
