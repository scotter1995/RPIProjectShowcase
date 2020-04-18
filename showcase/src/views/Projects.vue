<template>
  <div class="project_list" v-if="$route.path === '/projects'">
    <ProjectListPage v-bind:projects="project_list"/>
  </div>
  <div class="project" v-else>
    <ProjectPage v-bind:projects="project_list"/>
  </div>
</template>

<script>
import ProjectListPage from '../components/ProjectListPage.vue'
import ProjectPage from '../components/ProjectPage.vue'

export default {
  name: 'Projects',
  components: {
    ProjectListPage,
    ProjectPage
  },
  data() {
    return {
      project_list: [
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
        },
      ]
    }
  }
}
</script>