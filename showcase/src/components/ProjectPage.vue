<template>
    <div>
        <div v-bind:key="project.id" v-for="project in projects">
            <div v-if="$route.path === '/projects/' + project.title.trim().toLowerCase()">
                <h1>This is the {{project.title}} page</h1>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "ProjectPage",
    props: ["projects"]
}
</script>