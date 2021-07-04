<template>
  <section class="projects">
    <div class="projects-title">
      <h2>Projects</h2>
    </div>
    <div class="projects-content">
      <a
        v-for="project in projects"
        :key="project.name"
        href="#"
        class="projects-item"
      >
        <div class="project-item-text">
          <h2>{{ project.name }}</h2>
          <h3 class="subTitle">Read more about it</h3>
        </div>
        <img
          :src="require(`~/assets/img/${project.img}`)"
          :alt="project.alt"
          loading="lazy"
        />
      </a>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          name: 'Sockets',
          img: 'test2.webp',
          alt: 'Sockets project image',
        },
        {
          name: 'Trader',
          img: 'test.webp',
          alt: 'Trader project image',
        },
      ],
    }
  },
}
</script>
