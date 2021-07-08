<template>
  <div class="container">
    <section>
      <h1>{{ filteredProject.project }}</h1>
      <div class="project-image">
        <img
          :src="require(`~/assets/img/${filteredProject.img}`)"
          :alt="filteredProject.alt"
          loading="lazy"
        />
      </div>
      <p>{{ filteredProject.description }}</p>
      <span class="tag" v-for="i in filteredProject.tech">{{ i }}</span>
    </section>
  </div>
</template>

<script>
import projects from '../static/projects.json'
export default {
  async asyncData({ params, redirect }) {
    const Allprojects = projects.Projects

    const filteredProject = Allprojects.find(
      (el) => el.project === params.project
    )
    console.log(filteredProject)
    if (filteredProject) {
      return { filteredProject }
    } else {
      redirect('/')
    }
  }
}
</script>

<style scoped>
.project-image {
  height: 100%;
  max-height: 600px;
}

img {
  max-height: 600px;
}
</style>
