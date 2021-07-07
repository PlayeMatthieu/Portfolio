<template>
  <div>
    <h1>{{ filteredProject.Project }}</h1>
    <h2>{{ filteredProject.Img }}</h2>
  </div>
</template>

<script>
import projects from '../static/projects.json'
export default {
  async asyncData({ params, redirect }) {
    const Allprojects = projects.Projects

    const filteredProject = Allprojects.find(
      (el) => el.Project === params.project
    )
    console.log(filteredProject)
    if (filteredProject) {
      return { filteredProject }
    } else {
      redirect('/')
    }
  },
}
</script>
