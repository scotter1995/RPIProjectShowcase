<template>
    <div>
        <h1>This is the projects page</h1>
        <div v-bind:key="project.id" v-for="project in projects">
            <ProjectItem  v-bind:project="project"/>
        </div>
    </div>
</template>

<script>
import ProjectItem from "./Layout/ProjectItem.vue";

export default {
    name: "ProjectListPage",
    components: {
        ProjectItem
    },
    props: ["projects"]
}
</script>