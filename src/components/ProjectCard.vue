<template>
  <div class="flex">
    <div>
      <img :src="image" alt="project-image" >
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
  },
};
</script>

<style scoped lang="scss">
</style>
