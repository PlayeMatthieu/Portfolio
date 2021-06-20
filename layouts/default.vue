<template>
  <div>
    <!-- NAVBAR -->
    <navbarComponent />
    <!-- PAGE CONTENT -->
    <div class="container">
      <nuxt />
    </div>
    <!-- FOOTER -->
    <footerComponent />
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' },
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' },
        },
      ],
    }
  },
}
</script>
