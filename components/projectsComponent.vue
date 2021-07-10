<template>
  <section class="projects">
    <div class="projects-title">
      <h2>Projects</h2>
    </div>
    <div class="projects-content">
      <NuxtLink
        v-for="project in allProjects.Projects"
        :to="project.project"
        :key="project.project"
        href="#"
        class="projects-item"
        :class="project.heroImgClass"
      >
        <div class="project-item-text">
          <h2>{{ project.project }}</h2>
          <h3 class="subTitle">Read more about it</h3>
        </div>
        <!-- <img
          :src="require(`~/assets/img/${project.img}`)"
          :alt="project.alt"
          loading="lazy"
        /> -->
      </NuxtLink>
    </div>
  </section>
</template>

<script>
import projects from '../static/projects.json'
export default {
  data() {
    return {
      allProjects: projects,
    }
  },
}
</script>
