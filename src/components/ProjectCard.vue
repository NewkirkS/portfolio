<template>
  <div class="flex">
    <div>
      <img :src="imagePath" alt="project-image" >
    </div>
    <div>
      <h1>{{name}}</h1>
      <p>{{description}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectCard',
  props: {
    name: String,
    liveLink: String,
    repoLink: String,
    image: String,
    description: String,
    staticImagePath: String,
  },
  computed: {
    imagePath() {
      // eslint-disable-next-line global-require, import/no-dynamic-require
      return require(`../assets/${this.image}`);
    },
  },
};
</script>

<style scoped lang="scss">
</style>
