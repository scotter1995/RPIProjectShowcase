<template>
    <div class="project-item" v-bind:class="{'is-active':!project.active}">
        <h3>
            <img v-bind:alt="project.title + ' logo'" v-bind:src="require('../../assets/' + project.title.toLowerCase() + '_logo.png')" width = 400>
            <input type="button" v-on:click="markActive"> {{project.title}}
        </h3>
    </div>
</template>

<script>
export default {
    name: "ProjectItem",
    props: ["project"],
    methods: {
        markActive() {
            this.project.active = !this.project.active;
        }
    },
}
</script>

<style scoped>
.project-item {
    background: #f4f4f4;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}

.is-active {
    text-decoration: line-through;
}
</style>