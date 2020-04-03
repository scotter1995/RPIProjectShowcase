<template>
    <div class="project-item" v-bind:class="{'info':!project.active}">
        <h3>
        <img v-bind:alt="project.title + ' logo'" v-bind:src="require('../../assets/' + project.title.toLowerCase() + '.png')" width = 400>
            <input type="checkbox" v-on:change="markActive">
            {{project.title}}
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

.info {
    src: "../../assets/observatory.png";
}
</style>