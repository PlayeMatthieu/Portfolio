<template>
  <section class="container intro">
    <h3 v-html="content"></h3>
  </section>
</template>

<script>
export default {
  props: {
    content: String,
  },
}
</script>

<style scoped>
.intro {
  padding-top: 5em;
  padding-bottom: 5em;
}
h3 {
  color: #6b7280;
  text-align: center;
}
span {
  color: #000000;
}
</style>
