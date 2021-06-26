<template>
  <header class="header">
    <nav class="navbar">
      <a href="" class="nav-logo">Playe.be</a>
      <ul class="nav-menu">
        <li v-for="link in links" :key="link.title" class="nav-item">
          <a :href="link.href" class="nav-link" @click="closeNavbar">{{
            link.title
          }}</a>
        </li>
      </ul>
      <div class="hamburger" @click="toggleNavbar">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      links: [
        { title: 'Home', href: '#' },
        { title: 'About', href: '#' },
        { title: 'Contact', href: '#' },
      ],
    }
  },
  methods: {
    toggleNavbar: function () {
      const hamburger = document.querySelector('.hamburger')
      const navMenu = document.querySelector('.nav-menu')
      hamburger.classList.toggle('active')
      navMenu.classList.toggle('active')
    },
    closeNavbar: function () {
      const hamburger = document.querySelector('.hamburger')
      const navMenu = document.querySelector('.nav-menu')
      hamburger.classList.remove('active')
      navMenu.classList.remove('active')
    },
  },
}
</script>
