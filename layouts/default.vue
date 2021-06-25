<template>
  <div id="page-container">
    <div id="content-wrap">
      <navbarComponent />
      <nuxt class="container" />
    </div>
    <footerComponent id="footer" />
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style scoped>
#page-container {
  position: relative;
  min-height: 100vh;
}
#content-wrap {
  padding-bottom: 2.5rem; /* Footer height */
}
#footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 2.5rem; /* Footer height */
}
</style>
