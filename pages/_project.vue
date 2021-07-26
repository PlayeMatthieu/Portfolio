<template>
  <div class="container projectPage">
    <section>
      <h1>{{ filteredProject.project }}</h1>
      <div class="project-image" :class="filteredProject.heroImgClass"></div>
      <div class="pageDescriptionContainer">
        <p class="description" v-html="filteredProject.description">{{}}</p>
        <div class="tags">
          <p>Used technologies:</p>
          <span class="tag" v-for="i in filteredProject.tech">{{ i }}</span>
        </div>
      </div>
      <!-- <img
          :src="require(`~/assets/img/${filteredProject.img}`)"
          :alt="filteredProject.alt"
          loading="lazy"
        /> -->
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
    if (filteredProject) {
      return { filteredProject }
    } else {
      redirect('/')
    }
  },
}
</script>
