<template>
  <main>
    <heroComponent />
    <aboutComponent />
    <introTextComponent :content="text1" />
    <skillsComponent />
    <projectsComponent />
  </main>
</template>

<script>
export default {
  name: 'HomePage',
  data() {
    return {
      text1:
        'By programming application, I try to remove<br /><b>boring and repetitive tasks</b>',
    }
  },
}
</script>
