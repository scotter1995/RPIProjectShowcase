<template>
  <div class="projects">
    <h1>This is the projects page</h1>
    <ProjectPage v-bind:projects="projects"/>
  </div>
</template>

<script>
import ProjectPage from '../components/ProjectPage.vue'

export default {
  name: 'Projects',
  components: {
    ProjectPage
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Observatory",
          active: false
        },
        {
          id: 2,
          title: "Submitty",
          active: true
        },
        {
          id: 3,
          title: "YACS",
          active: true
        }
      ]
    }
  }
}
</script>